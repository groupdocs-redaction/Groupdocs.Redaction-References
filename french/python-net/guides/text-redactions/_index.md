---
title: "Censure de texte"
linkTitle: "Text redaction"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Cet article explique comment l'API de censure Python vous permet de censurer facilement les données sensibles ou privées de vos documents. Vous pouvez appliquer la censure de texte en utilisant une phrase exacte ou une expression régulière pour des documents de différents formats tels que PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX et autres."
type: docs
url: /fr/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction permet de censurer facilement les données sensibles ou privées de vos documents. Le cas de censure le plus courant consiste à supprimer un texte d'un document.

Avec l'API GroupDocs.Redaction, vous pouvez appliquer la censure de texte en utilisant une phrase exacte ou [une expression régulière](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) pour des documents de différents formats tels que PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX et autres. Consultez la liste complète dans l'article [formats de documents pris en charge]().

## Use exact phrase redaction

Dans l'exemple ci‑dessous, nous appliquons une censure textuelle, en remplaçant la phrase exacte personnelle "John Doe" par "\[personal\]" (ou tout code d'exemption) :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # Spécifiez les options de redaction
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Chargez le document à censurer
    with Redactor("./sample.docx") as redactor:
        # Appliquer le masquage
        result = redactor.apply(ex_red)

        # Enregistrez le document masqué à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) pour le télécharger.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

Par défaut, la recherche de la phase exacte est insensible à la casse. Pour une rédaction sensible à la casse, il existe un paramètre du constructeur et une propriété publique correspondante :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # Activer la correspondance sensible à la casse
    case_sensitive = True

    # Spécifiez les options de redaction
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # Chargez le document à censurer
    with Redactor("./sample.docx") as redactor:
        # Appliquer le masquage
        result = redactor.apply(ex_red)

        # Enregistrez le document masqué à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) pour le télécharger.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

Si vous avez besoin d’une boîte colorée au-dessus du texte masqué, vous pouvez utiliser la couleur à la place de la chaîne de remplacement. La rédaction effacera le texte correspondant et placera un rectangle de la couleur spécifiée à la place du texte masqué :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # Définir la couleur de la boîte de rédaction
    color = Color.from_argb(255, 220, 20, 60)

    # Spécifiez les options de redaction
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Chargez le document à censurer
    with Redactor("./sample.docx") as redactor:
        # Appliquer le masquage
        result = redactor.apply(ex_red)

        # Enregistrez le document masqué à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) pour le télécharger.

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

Il se peut que vous deviez appliquer une rédaction à un document de droite à gauche, tel que l’arabe ou l’hébreu. L’exemple suivant montre comment appliquer ExactPhraseRedaction à un document PDF en arabe :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # Spécifiez les options de rédaction avec une phrase en arabe
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # Chargez le document à censurer
    with Redactor("./arabic.pdf") as redactor:
        # Appliquer le masquage
        result = redactor.apply(ex_red)

        # Enregistrez le document masqué à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` est le fichier d’exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) pour le télécharger.

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

En coulisses, la rédaction "exact phrase" fonctionne grâce aux expressions régulières, qui constituent l’approche de base pour la rédaction. Dans l’exemple ci‑dessous, nous masquons tout texte correspondant à "2 chiffres, espace ou rien, 2 chiffres, à nouveau espace et 6 chiffres" avec une boîte de couleur bleue :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # Définir la couleur de la boîte de rédaction
    color = Color.from_argb(255, 220, 20, 60)

    # Spécifiez les options de redaction
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # Chargez le document à censurer
    with Redactor("./sample.docx") as redactor:
        # Appliquer le masquage
        result = redactor.apply(reg_red)

        # Enregistrez le document masqué à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) pour le télécharger.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

Si vous devez appliquer une rédaction à un paragraphe entier, vous pourriez également devoir utiliser RegexRedaction. L’exemple suivant montre comment masquer tout le paragraphe dans un document PDF :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # Définir la couleur de la boîte de rédaction
    color = Color.from_argb(255, 220, 20, 60)

    # Spécifiez les options de rédaction qui correspondent à un paragraphe entier
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # Chargez le document à censurer
    with Redactor("./sample.pdf") as redactor:
        # Appliquer le masquage
        result = redactor.apply(reg_red)

        # Enregistrez le document masqué à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` est le fichier d’exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) pour le télécharger.

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
