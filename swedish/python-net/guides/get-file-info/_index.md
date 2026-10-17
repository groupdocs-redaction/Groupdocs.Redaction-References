---
title: "Hämta filinformation"
linkTitle: "Get file info"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Denna artikel förklarar GroupDocs.Redaction API:s förmåga att hämta generell dokumentinformation, som inkluderar FileType, PageCount och FileSize."
type: docs
url: /sv/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction tillhandahåller generell dokumentinformation, som inkluderar:

*   FileType
*   PageCount
*   FileSize

Följande kodexempel visar hur man hämtar dokumentinformation.

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # Läs in dokumentet från lokal disk
    with Redactor("./sample.docx") as redactor:
        # Hämta generell dokumentinformation
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` är exempelfilen som används i detta exempel. Klicka [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) för att ladda ner den.

  
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
    # Öppna dokumentet som en binär ström
    with open("./sample.docx", "rb") as stream:
        # Läs in dokumentet från strömmen
        with Redactor(stream) as redactor:
            # Hämta generell dokumentinformation
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` är exempelfilen som används i detta exempel. Klicka [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) för att ladda ner den.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
