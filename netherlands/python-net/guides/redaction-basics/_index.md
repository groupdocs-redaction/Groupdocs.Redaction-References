---
title: "Basisprincipes van redactie"
linkTitle: "Redaction basics"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Dit artikel laat zien hoe Python‑ontwikkelaars metadata, afbeeldingen, annotaties en tekstredactie in hun documenten kunnen toepassen. Een breed scala aan documentformaten wordt ondersteund, zoals PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX en andere."
type: docs
url: /nl/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


GroupDocs.Redaction ondersteunt een effectief pakket aan documentredactie‑functies. Het maakt het mogelijk om redacties toe te passen op [text](), [metadata](), [annotations](), [images]().

Een breed scala aan documentformaten wordt ondersteund, zoals: PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX en andere. Zie de volledige lijst met ondersteunde formaten in het artikel [supported document formats]().

## Redaction types

GroupDocs.Redaction wordt geleverd met de volgende redactietypen:

| Type | Beschrijving | Klassen |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

Het toepassen van redactie op een document gebeurt via de methode [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/). Als resultaat ontvang je een instantie van [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) die een logboekvermelding bevat voor elke toegepaste redactie. De vermelding bevat een verwijzing naar de [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/)‑instantie inclusief de opties, de status van de bewerking (zie hieronder) en tekstuele beschrijvingen indien van toepassing. Als minstens één redactie is mislukt, zie je [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # Specificeer de redactie‑opties
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Laad het te redigeren document
    with Redactor("./sample.docx") as redactor:
        # Pas de redactie toe
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # Sla het geredigeerde document op naast het bronbestand
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik op [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) om het te downloaden.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

Alle mogelijke statussen van de enumeratie [RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) worden in deze tabel weergegeven:

| Status | Beschrijving | Mogelijke redenen |
| --- | --- | --- |
| *Applied* | Redactie is volledig en succesvol toegepast | Alle bewerkingen binnen het redactieproces zijn succesvol toegepast |
| *PartiallyApplied* | Redactie is alleen op een deel van de overeenkomsten toegepast | 1) Proefbeperkingen voor vervangingen zijn overschreden2) Ten minste één wijziging is door de gebruiker afgewezen |
| *Skipped* | Redactie is overgeslagen (niet toegepast) | 1) Proefbeperkingen voor redacties zijn overschreden2) Redactie kan niet op dit type document worden toegepast3) Alle vervangingen zijn door de gebruiker afgewezen en er zijn geen wijzigingen aangebracht |
| *Failed* | Redactie is mislukt met een uitzondering | Er trad een uitzondering op tijdens het redactieproces |

Voor gedetailleerde informatie moet je door de logboekvermeldingen van redactie itereren in [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) en de eigenschap [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) controleren van alle items met een status anders dan *Applied*:

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # Standaard wordt het geredigeerde document opgeslagen in PDF-formaat
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # Dump alle mislukte of overgeslagen redacties
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

Je kunt zoveel redacties toepassen als nodig in één aanroep van de methode [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) omdat de overload een array van redacties en een redactiebeleid accepteert. In dit geval worden de redacties toegepast in dezelfde volgorde als ze in de array staan. Als alternatief voor het specificeren van redactiesets in je code, kun je een XML‑bestand met redactiebeleid maken, zoals beschreven [here]().

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
    # Definieer de kleur van de redactiedoos
    color = Color.from_argb(255, 220, 20, 60)

    # Geef een lijst met redacties op die in volgorde moeten worden toegepast
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Laad het te redigeren document
    with Redactor("./sample.docx") as redactor:
        # Pas de lijst met redacties toe
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # Standaard wordt het geredigeerde document opgeslagen in PDF-formaat
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # Dump alle mislukte of overgeslagen redacties
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik op [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) om het te downloaden.

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
