---
title: "Dapatkan info file"
linkTitle: "Get file info"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Artikel ini menjelaskan kemampuan API GroupDocs.Redaction untuk mendapatkan informasi umum dokumen, yang mencakup FileType, PageCount, dan FileSize."
type: docs
url: /id/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction menyediakan informasi umum dokumen, yang mencakup:

*   FileType
*   PageCount
*   FileSize

Contoh kode berikut menunjukkan cara mendapatkan informasi dokumen.

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # Muat dokumen dari disk lokal
    with Redactor("./sample.docx") as redactor:
        # Ambil informasi umum dokumen
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) untuk mengunduhnya.

  
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
    # Buka dokumen sebagai aliran biner
    with open("./sample.docx", "rb") as stream:
        # Muat dokumen dari aliran
        with Redactor(stream) as redactor:
            # Ambil informasi umum dokumen
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) untuk mengunduhnya.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
