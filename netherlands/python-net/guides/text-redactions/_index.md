---
title: "Tekstredactie"
linkTitle: "Text redaction"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Dit artikel legt uit hoe de Python redacties API je in staat stelt om eenvoudig gevoelige of privégegevens uit je documenten te redigeren. Je kunt tekstredactie toepassen met een exacte zin of reguliere expressie voor documenten in verschillende formaten zoals PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX en andere."
type: docs
url: /nl/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction maakt het eenvoudig om gevoelige of privégegevens uit je documenten te redigeren. Het meest voorkomende redactiescenario is het verwijderen van tekst uit een document.

Met de GroupDocs.Redaction API kun je tekstredactie toepassen met een exacte zin of [reguliere expressie](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) voor documenten in verschillende formaten zoals PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX en andere. Zie de volledige lijst in het artikel [ondersteunde documentformaten]().

## Use exact phrase redaction

In het onderstaande voorbeeld passen we tekstredactie toe, waarbij we de persoonlijke exacte zin "John Doe" vervangen door "\[personal\]" (of een andere vrijstellingscode):

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # Specificeer de redactie‑opties
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Laad het te redigeren document
    with Redactor("./sample.docx") as redactor:
        # Pas de redactie toe
        result = redactor.apply(ex_red)

        # Sla het geredigeerde document op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) om het te downloaden.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

Standaard is zoeken naar exacte fase hoofdletterongevoelig. Voor een hoofdlettergevoelige redactie is er een constructorparameter en bijbehorende openbare eigenschap:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # Schakel hoofdlettergevoelige overeenstemming in
    case_sensitive = True

    # Specificeer de redactie‑opties
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # Laad het te redigeren document
    with Redactor("./sample.docx") as redactor:
        # Pas de redactie toe
        result = redactor.apply(ex_red)

        # Sla het geredigeerde document op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) om het te downloaden.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

Als u een gekleurde doos over de geredigeerde tekst nodig heeft, kunt u kleur gebruiken in plaats van een vervangingsreeks. De redactie zal de overeenkomende tekst wissen en een rechthoek van de opgegeven kleur op de plaats van de geredigeerde tekst plaatsen:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # Definieer de kleur van de redactiedoos
    color = Color.from_argb(255, 220, 20, 60)

    # Specificeer de redactie‑opties
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Laad het te redigeren document
    with Redactor("./sample.docx") as redactor:
        # Pas de redactie toe
        result = redactor.apply(ex_red)

        # Sla het geredigeerde document op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) om het te downloaden.

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

U moet mogelijk redactie toepassen op een rechts-naar-links document, zoals Arabisch of Hebreeuws. Het volgende voorbeeld laat zien hoe u ExactPhraseRedaction toepast op een Arabisch PDF‑document:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # Specificeer de redactiemogelijkheden met een Arabische zin
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # Laad het te redigeren document
    with Redactor("./arabic.pdf") as redactor:
        # Pas de redactie toe
        result = redactor.apply(ex_red)

        # Sla het geredigeerde document op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) om het te downloaden.

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

Achter de schermen werkt "exacte zin" redactie via reguliere expressies, die de basisaanpak voor redactie vormen. In het onderstaande voorbeeld verwijderen we elke tekst die overeenkomt met "2 cijfers, spatie of niets, 2 cijfers, opnieuw spatie en 6 cijfers" met een blauwe gekleurde doos:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # Definieer de kleur van de redactiedoos
    color = Color.from_argb(255, 220, 20, 60)

    # Specificeer de redactie‑opties
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # Laad het te redigeren document
    with Redactor("./sample.docx") as redactor:
        # Pas de redactie toe
        result = redactor.apply(reg_red)

        # Sla het geredigeerde document op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) om het te downloaden.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

Als u een hele alinea moet redigeren, moet u mogelijk ook RegexRedaction gebruiken. Het volgende voorbeeld laat zien hoe u de volledige alinea in een PDF‑document redigeert:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # Definieer de kleur van de redactiedoos
    color = Color.from_argb(255, 220, 20, 60)

    # Specificeer de redactiemogelijkheden die een volledige alinea overeenkomen
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # Laad het te redigeren document
    with Redactor("./sample.pdf") as redactor:
        # Pas de redactie toe
        result = redactor.apply(reg_red)

        # Sla het geredigeerde document op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) om het te downloaden.

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
