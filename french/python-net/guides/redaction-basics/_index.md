---
title: "Notions de base sur la rédaction"
linkTitle: "Redaction basics"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Cet article montre comment les développeurs Python peuvent appliquer la rédaction de métadonnées, d’images, d’annotations et de texte dans leurs documents. Un large éventail de formats de documents est pris en charge, tels que PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX et autres."
type: docs
url: /fr/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


GroupDocs.Redaction prend en charge un ensemble efficace de fonctionnalités de rédaction de documents. Il permet d’appliquer des rédactions pour [text](), [metadata](), [annotations](), [images]().

Un large éventail de formats de documents est pris en charge, tels que : PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX et autres. Consultez la liste complète des formats pris en charge dans l’article [supported document formats]().

## Redaction types

GroupDocs.Redaction propose les types de rédaction suivants :

| Type | Description | Classes |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

L'application d'une rédaction à un document se fait via la méthode [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) . En conséquence, vous recevez une instance [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) contenant une entrée de journal pour chaque rédaction appliquée. L'entrée contient une référence à l'instance [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/) incluant ses options, le statut de l'opération (voir ci-dessous) et les descriptions textuelles le cas échéant. Si au moins une rédaction a échoué, vous verrez [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # Spécifiez les options de redaction
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Chargez le document à censurer
    with Redactor("./sample.docx") as redactor:
        # Appliquer le masquage
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # Enregistrez le document masqué à côté du fichier source
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez sur [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) pour le télécharger.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

Tous les statuts possibles de l'énumération [RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) sont répertoriés dans ce tableau :

| Statut | Description | Raisons possibles |
| --- | --- | --- |
| *Appliqué* | La rédaction a été entièrement et avec succès appliquée | Toutes les opérations du processus de rédaction ont été appliquées avec succès |
| *PartiellementAppliqué* | La rédaction n'a été appliquée qu'à une partie de ses correspondances | 1) Les limites d'essai pour les remplacements ont été dépassées2) Au moins une modification a été rejetée par l'utilisateur |
| *Ignoré* | La rédaction a été ignorée (non appliquée) | 1) Les limites d'essai pour les rédactions ont été dépassées2) La rédaction ne peut pas être appliquée à ce type de document3) Toutes les remplacements ont été rejetées par l'utilisateur et aucune modification n'a été effectuée |
| *Échoué* | La rédaction a échoué avec une exception | Une exception s'est produite lors du processus de rédaction |

Pour obtenir des informations détaillées, vous devez parcourir les entrées du journal de rédaction dans [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) et vérifier la propriété [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) de tout élément dont le statut n'est pas *Appliqué* :

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # Par défaut, le document redacté est enregistré au format PDF
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # Exporter toutes les rédactions échouées ou ignorées
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

Vous pouvez appliquer autant de rédactions que nécessaire en un seul appel à la méthode [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) , car sa surcharge accepte un tableau de rédactions et une politique de rédaction. Dans ce cas, les rédactions seront appliquées dans le même ordre qu'elles apparaissent dans le tableau. En alternative à la spécification des ensembles de rédaction dans votre code, vous pouvez créer un fichier XML avec la politique de rédaction, comme décrit [ici]().

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    ReplacementOptions,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def apply_multiple_redactions():
    # Définir la couleur de la boîte de rédaction
    color = Color.from_argb(255, 220, 20, 60)

    # Fournissez une liste de rédactions à appliquer dans l'ordre
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Chargez le document à censurer
    with Redactor("./sample.docx") as redactor:
        # Appliquer la liste des rédactions
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # Par défaut, le document redacté est enregistré au format PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # Exporter toutes les rédactions échouées ou ignorées
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez sur [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) pour le télécharger.

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
