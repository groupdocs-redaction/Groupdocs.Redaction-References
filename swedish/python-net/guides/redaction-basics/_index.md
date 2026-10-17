---
title: "Grundläggande om redigering"
linkTitle: "Redaction basics"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Denna artikel visar hur Python-utvecklare kan tillämpa metadata-, bild-, annoterings- och textredigering i sina dokument. Ett brett sortiment av dokumentformat stöds, såsom PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX och andra."
type: docs
url: /sv/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


GroupDocs.Redaction stöder en effektiv uppsättning funktioner för dokumentredigering. Det möjliggör att tillämpa redigeringar för [text](), [metadata](), [annotations](), [images]().

Ett brett sortiment av dokumentformat stöds, såsom: PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX och andra. Se den fullständiga listan över stödda format i artikeln [supported document formats]().

## Redaction types

GroupDocs.Redaction levereras med följande redigeringstyper:

| Typ | Beskrivning | Klasser |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

Att tillämpa maskering på ett dokument görs via metoden [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) . Som resultat får du en [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/)‑instans som innehåller en loggpost för varje tillämpad maskering. Posten innehåller en referens till [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/)‑instansen inklusive dess alternativ, operationens status (se nedan) och textbeskrivningar när det är tillämpligt. Om minst en maskering misslyckades kommer du att se [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # Ange redigeringsalternativen
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.docx") as redactor:
        # Applicera maskeringen
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # Spara det redigerade dokumentet bredvid källfilen
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) för att ladda ner den.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

Alla möjliga statusar för uppräkningen [RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) listas i denna tabell:

| Status | Beskrivning | Möjliga orsaker |
| --- | --- | --- |
| *Applied* | Maskeringen tillämpades fullt ut och framgångsrikt | Alla operationer inom maskeringsprocessen tillämpades framgångsrikt |
| *PartiallyApplied* | Maskeringen tillämpades endast på en del av dess matchningar | 1) Provtidsbegränsningar för ersättningar överskreds2) Minst en ändring avvisades av användaren |
| *Skipped* | Maskeringen hoppades över (inte tillämpad) | 1) Provtidsbegränsningar för maskeringar överskreds2) Maskering kan inte tillämpas på den här dokumenttypen3) Alla ersättningar avvisades av användaren och inga ändringar gjordes |
| *Failed* | Maskeringen misslyckades med ett undantag | Ett undantag inträffade i maskeringsprocessen |

För detaljerad information måste du iterera genom maskeringsloggposter i [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) och kontrollera egenskapen [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) för alla objekt med status annat än *Applied*:

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # Som standard sparas det maskerade dokumentet i PDF-format
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # Exportera alla misslyckade eller hoppade över maskeringar
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

Du kan tillämpa så många rödaktioner du behöver i ett enda anrop till [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) metoden, eftersom dess överlagring accepterar en array av rödaktioner och rödaktionspolicy. I detta fall kommer rödaktionerna att tillämpas i samma ordning som de förekommer i arrayen. Som ett alternativ till att specificera rödaktionsuppsättningar i din kod kan du skapa en XML-fil med rödaktionspolicy, som beskrivs [här]().

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
    # Definiera färgen på redigeringsrutan
    color = Color.from_argb(255, 220, 20, 60)

    # Tillhandahåll en lista med rödaktioner att tillämpa i ordning
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.docx") as redactor:
        # Tillämpa listan med rödaktioner
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # Som standard sparas det maskerade dokumentet i PDF-format
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # Exportera alla misslyckade eller hoppade över maskeringar
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) för att ladda ner den.

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
