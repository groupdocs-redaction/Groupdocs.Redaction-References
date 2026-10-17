---
title: "Metadaten‑Redaktionen"
linkTitle: "Metadata redactions"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Dieser Artikel zeigt, wie die Python‑Redaction‑API es Ihnen ermöglicht, Metadaten mithilfe von Filtern oder regulären Ausdrücken zu ersetzen oder zu entfernen."
type: docs
url: /de/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


Mit der GroupDocs.Redaction‑API können Sie Metadaten‑Redaktionen für Dokumente verschiedener Formate wie PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX und andere anwenden. Siehe die vollständige Liste im Artikel [supported document formats]().

GroupDocs.Redactions bietet eine flexible API, die das Ersetzen oder Entfernen von Metadaten mithilfe von Filtern oder regulären Ausdrücken ermöglicht.

## Filter metadata

Die Grundfunktionalität für alle Redaktionen, abgeleitet von der Basisklasse [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/), ist *metadata filtering* und ist für Metadaten‑Redaktionen obligatorisch. Sie verwendet die gekennzeichnete Aufzählung [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/), die Elemente für die häufigsten Metadaten‑Einträge enthält. Sie können den Filter auf *All* setzen oder eine beliebige Kombination von Metadaten wählen. Zum Beispiel setzt das untenstehende Beispiel den Filter auf *Author*, *Manager* und *NameOfApplication* – für textuelle Redaktion oder deren Bereinigung:

```python
# Redaktion abgeleitet von MetadataRedaction
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

Unten ist die Tabelle mit der vollständigen Liste der [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/)‑Elemente:

| Filter | Numerischer Wert | Beschreibung |
| --- | --- | --- |
| *None* | 0 | Leere Filtereinstellung, trifft auf keine Metadaten‑Einträge zu |
| *Author* | 1 | Autor des Dokuments |
| *Kategorie* | 2 | Kategorie des Dokuments |
| *Kommentare* | 4 | Dokumentkommentar |
| *Firma* | 8 | Firma des Autors |
| *ContentStatus* | 16 | Inhaltsstatus |
| *CreatedTime* | 32 | Erstellungszeit |
| *HyperlinkBase* | 64 | Hyperlink-Basis |
| *LastPrinted* | 128 | Datum und Uhrzeit des letzten Drucks |
| *LastSavedBy* | 256 | Zuletzt vom Benutzer gespeichert |
| *LastSavedTime* | 1024 | Datum und Uhrzeit der letzten Speicherung |
| *NameOfApplication* | 2048 | Name der Anwendung, in der das Dokument erstellt wurde |
| *Manager* | 4096 | Name des Managers des Autors |
| *RevisionNumber* | 8192 | Revisionsnummer |
| *Subject* | 16384 | Betreff des Dokuments |
| *Template* | 32768 | Name der Dokumentvorlage |
| *Title* | 65536 | Dokumenttitel |
| *TotalEditingTime* | 131072 | Gesamte Bearbeitungszeit |
| *Version* | 262144 | Version des Dokuments |
| *Beschreibung* | 524288 | Beschreibung des Dokuments |
| *Schlüsselwörter* | 1048576 | Schlüsselwörter des Dokuments |
| *ContentType* | 2097152 | Inhaltstyp |
| *Alle* | 2147483647 | Alle Arten von Metadaten-Elementen |

## Clean metadata

Sie können alle oder bestimmte Metadaten im Dokument durch leere (leere oder minimale) Werte ersetzen, indem Sie die Klasse [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) verwenden. Das folgende Beispiel leert alle Eigenschaften des Dokuments:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # Geben Sie die Redaktionsoptionen an, um alle Metadaten zu löschen
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.docx") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(met_red)

        # Speichern Sie das redigierte Dokument neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx), um sie herunterzuladen.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

Sie können [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) angeben oder den Standardkonstruktor verwenden, um alle Metadaten im angegebenen Dokument zu leeren, Custom – um alle benutzerdefinierten Metadaten‑Einträge zu löschen.

## Redact metadata

Sie können [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) verwenden, um sensible Daten aus den Metadaten des Dokuments mithilfe regulärer Ausdrücke zu entfernen. Zum Beispiel können wir jede Erwähnung von "Company Ltd." entfernen:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # Geben Sie die Redaktionsoptionen an: Suchmuster und Ersetzungszeichenfolge
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.docx") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(met_red)

        # Speichern Sie das redigierte Dokument neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx), um sie herunterzuladen.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

Das erste Argument ist ein regulärer Ausdruck, das zweite eine Ersetzungszeichenfolge. Sie können den Geltungsbereich der Redaktion auch festlegen, indem Sie einen Filter setzen, z. B. auf [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/). – dies lässt die Übereinstimmungen der regulären Ausdrücke in allen Metadaten‑Elementen unverändert, außer bei der Eigenschaft "Company":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # Geben Sie die Redaktionsoptionen an: Suchmuster und Ersetzungszeichenfolge
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Beschränken Sie den Redaktionsbereich ausschließlich auf das Metadaten‑Element Company
    met_red.filter = MetadataFilters.COMPANY

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.docx") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(met_red)

        # Speichern Sie das redigierte Dokument neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx), um sie herunterzuladen.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

Alle Metadaten‑Redaktionen werden auf jedes Metadaten‑Element einzeln angewendet, und selbst wenn die Redaktion eines Elements fehlschlägt, werden die übrigen Metadaten‑Elemente aktualisiert. Eine Liste fehlgeschlagener, übersprungener (abgelehnter) Metadaten‑Elemente und die Gründe dafür finden Sie in der Eigenschaft [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) von [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).
