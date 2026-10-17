---
title: "Grundlagen der Redaktion"
linkTitle: "Redaction basics"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Dieser Artikel zeigt, wie Python-Entwickler Metadaten-, Bild-, Anmerkungs- und Textredaktionen in ihren Dokumenten anwenden können. Ein breites Spektrum an Dokumentformaten wird unterstützt, wie z. B. PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX und andere."
type: docs
url: /de/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


**GroupDocs.Redaction** unterstützt ein effektives Set an Dokument-Redaktions-Funktionen. Es ermöglicht das Anwenden von Redaktionen für [text](), [metadata](), [annotations](), [images]().

Ein breites Spektrum an Dokumentformaten wird unterstützt, wie: PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX und andere. Die vollständige Liste der unterstützten Formate finden Sie im Artikel [supported document formats]().

## Redaction types

**GroupDocs.Redaction** bietet die folgenden Redaktionstypen:

| Typ | Beschreibung | Klassen |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

Das Anwenden einer Redaktion auf ein Dokument erfolgt über die Methode [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/). Als Ergebnis erhalten Sie eine Instanz von [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/), die einen Protokolleintrag für jede angewendete Redaktion enthält. Der Eintrag enthält eine Referenz zur Instanz [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/), einschließlich ihrer Optionen, des Status der Operation (siehe unten) und textuelle Beschreibungen, falls zutreffend. Wenn mindestens eine Redaktion fehlgeschlagen ist, sehen Sie [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # Geben Sie die Redaktionsoptionen an
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.docx") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # Speichern Sie das redigierte Dokument neben der Quelldatei
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) zum Herunterladen.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

Alle möglichen Status der Aufzählung [RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) werden in dieser Tabelle aufgeführt:

| Status | Beschreibung | Mögliche Gründe |
| --- | --- | --- |
| *Applied* | Die Redaktion wurde vollständig und erfolgreich angewendet | Alle Vorgänge im Redaktionsprozess wurden erfolgreich angewendet |
| *PartiallyApplied* | Die Redaktion wurde nur auf einen Teil ihrer Treffer angewendet | 1) Die Testbeschränkungen für Ersetzungen wurden überschritten2) Mindestens eine Änderung wurde vom Benutzer abgelehnt |
| *Skipped* | Die Redaktion wurde übersprungen (nicht angewendet) | 1) Die Testbeschränkungen für Redaktionen wurden überschritten2) Die Redaktion kann auf diesen Dokumenttyp nicht angewendet werden3) Alle Ersetzungen wurden vom Benutzer abgelehnt und es wurden keine Änderungen vorgenommen |
| *Failed* | Redaktion fehlgeschlagen mit Ausnahme | Im Verlauf der Redaktion ist eine Ausnahme aufgetreten |

Für detaillierte Informationen müssen Sie die Einträge des Redaktionsprotokolls in [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) durchlaufen und die Eigenschaft [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) von allen Elementen prüfen, deren Status nicht *Applied* ist:

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # Standardmäßig wird das redigierte Dokument im PDF-Format gespeichert.
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # Alle fehlgeschlagenen oder übersprungenen Redaktionen ausgeben
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

Sie können beliebig viele Redaktionen in einem einzigen Aufruf der Methode [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) anwenden, da deren Überladung ein Array von Redaktionen und eine Redaktionsrichtlinie akzeptiert. In diesem Fall werden die Redaktionen in derselben Reihenfolge angewendet, in der sie im Array erscheinen. Als Alternative zur Angabe von Redaktionssätzen im Code können Sie eine XML-Datei mit Redaktionsrichtlinie erstellen, wie [hier](). beschrieben.

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
    # Definieren Sie die Farbe der Redaktions-Box
    color = Color.from_argb(255, 220, 20, 60)

    # Geben Sie eine Liste von Redaktionen an, die in der gewünschten Reihenfolge angewendet werden sollen
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.docx") as redactor:
        # Wenden Sie die Liste der Redaktionen an
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # Standardmäßig wird das redigierte Dokument im PDF-Format gespeichert.
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # Alle fehlgeschlagenen oder übersprungenen Redaktionen ausgeben
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) zum Herunterladen.

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
