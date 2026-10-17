---
title: "Dateiinformationen abrufen"
linkTitle: "Get file info"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Dieser Artikel erklärt die Fähigkeit der GroupDocs.Redaction‑API, allgemeine Dokumentinformationen abzurufen, die Dateityp, Seitenzahl und Dateigröße umfassen."
type: docs
url: /de/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction liefert allgemeine Dokumentinformationen, die Folgendes umfassen:

*   FileType
*   PageCount
*   FileSize

Die folgenden Codebeispiele zeigen, wie man Dokumentinformationen abruft.

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # Laden Sie das Dokument von der lokalen Festplatte
    with Redactor("./sample.docx") as redactor:
        # Allgemeine Dokumentinformationen abrufen
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx), um sie herunterzuladen.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_local_file_info/get-local-file-info.txt)

## Get file info for a file from Stream

```python
from groupdocs.redaction import Redactor

def get_file_info_from_stream():
    # Öffnen Sie das Dokument als Binär-Stream
    with open("./sample.docx", "rb") as stream:
        # Laden Sie das Dokument aus dem Stream
        with Redactor(stream) as redactor:
            # Allgemeine Dokumentinformationen abrufen
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx), um sie herunterzuladen.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
