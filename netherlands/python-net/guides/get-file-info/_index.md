---
title: "Bestandsinformatie ophalen"
linkTitle: "Get file info"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Dit artikel legt de mogelijkheid van de GroupDocs.Redaction API uit om algemene documentinformatie op te halen, waaronder FileType, PageCount en FileSize."
type: docs
url: /nl/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction biedt algemene documentinformatie, die omvat:

*   FileType
*   PageCount
*   FileSize

De volgende codevoorbeelden laten zien hoe je documentinformatie kunt ophalen.

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # Laad het document vanaf de lokale schijf
    with Redactor("./sample.docx") as redactor:
        # Haal algemene documentinformatie op
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik op [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) om het te downloaden.

  
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
    # Open het document als een binaire stream
    with open("./sample.docx", "rb") as stream:
        # Laad het document vanuit de stream
        with Redactor(stream) as redactor:
            # Haal algemene documentinformatie op
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik op [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) om het te downloaden.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
