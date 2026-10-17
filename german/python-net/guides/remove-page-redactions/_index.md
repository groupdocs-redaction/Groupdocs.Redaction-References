---
title: "Seitenredaktionen entfernen"
linkTitle: "Remove page redactions"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Dieser Artikel zeigt, wie man Seiten mit sensiblen Daten aus Ihren PDF-, Präsentations- und Tabellenkalkulationsdokumenten entfernt."
type: docs
url: /de/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction ermöglicht das einfache Entfernen von Seiten aus PDF-Dokumenten, Folien aus Präsentationen und Arbeitsblättern aus Tabellenkalkulationsdokumenten.

Mit der GroupDocs.Redaction API können Sie Seiten entfernen, indem Sie den Seitenbereich über seine relative Position (Anfang oder Ende), den nullbasierten Index und die Anzahl der zu entfernenden Seiten angeben. Derzeit unterstützte Formate sind: PDF, Präsentationen (Microsoft PowerPoint, OpenOffice Präsentationen), Textverarbeitungsdokumente (Microsoft Word, OpenOffice Texte, Rich-Text-Dateien), Tabellenkalkulationen (Microsoft Excel, OpenOffice Tabellen, usw.) und Mehrbild- (Multi-Frame-) Bilder.

## Remove page range

Im folgenden Beispiel entfernen wir die 2., 3. und 4. Seite aus dem Dokument, sofern das Dokument genügend Seiten enthält:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # Laden Sie das zu redigierende Dokument
    with Redactor("./multipage_sample.pdf") as redactor:
        # Dokumentinformationen abrufen
        doc_info = redactor.get_document_info()

        # Erfordert mindestens 4 Seiten
        if doc_info.page_count > 3:
            # Entferne 3 Seiten ab der 2. Seite (nullbasierter Index 1)
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # Wende die Schwärzung an
            result = redactor.apply(rem_opt)

            # Speichern Sie das redigierte Dokument neben der Quelldatei
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` ist die in diesem Beispiel verwendete Beispieldatei. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf), um sie herunterzuladen.

## Remove last page

In manchen Fällen müssen Sie möglicherweise die letzte Seite oder mehrere Seiten löschen, unabhängig davon, wie viele Seiten vorhanden sind.

Das folgende Beispiel zeigt, wie man die letzte Seite aus einem Dokument entfernt:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Entferne 1 Seite, gezählt vom Ende des Dokuments
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # Laden Sie das zu redigierende Dokument
    with Redactor("./multipage_sample.pdf") as redactor:
        # Dokumentinformationen abrufen
        doc_info = redactor.get_document_info()

        # Erfordert mindestens 2 Seiten, damit das Dokument nicht leer bleibt
        if doc_info.page_count > 1:
            # Wende die Schwärzung an
            result = redactor.apply(rem_opt)

            # Speichern Sie das redigierte Dokument neben der Quelldatei
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` ist die in diesem Beispiel verwendete Beispieldatei. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf), um sie herunterzuladen.

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

Im Falle eines Mehrbild- (Multi-Frame-) Bildes müssen Sie möglicherweise mehrere Frames (als \"pages\" behandelt) löschen.

Das folgende Beispiel zeigt, wie man 3 Frames aus einem animierten GIF‑Bild entfernt:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # Entferne Frames ab dem 3. Frame (nullbasierter Index 2)
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # Laden Sie das zu redigierende Mehrbild‑Bild
    with Redactor("./sample.gif") as redactor:
        # Dokumentinformationen abrufen
        doc_info = redactor.get_document_info()

        # Erfordert mindestens 7 Frames
        if doc_info.page_count >= 7:
            # Wende die Schwärzung an
            result = redactor.apply(rem_opt)

            # Speichern Sie das redigierte Bild neben der Quelldatei
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` ist die in diesem Beispiel verwendete Beispieldatei. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif), um sie herunterzuladen.

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)
