---
title: "Dosya bilgilerini al"
linkTitle: "Get file info"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bu makale, GroupDocs.Redaction API'sinin dosya türü, sayfa sayısı ve dosya boyutu gibi genel belge bilgilerini alabilme yeteneğini açıklar."
type: docs
url: /tr/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction, aşağıdakileri içeren genel belge bilgileri sağlar:

*   FileType
*   PageCount
*   FileSize

Aşağıdaki kod örnekleri belge bilgilerini nasıl alacağınızı gösterir.

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # Belgeyi yerel diskinizden yükleyin
    with Redactor("./sample.docx") as redactor:
        # Genel belge bilgilerini alın
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) tıklayın.

  
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
    # Belgeyi ikili akış olarak açın
    with open("./sample.docx", "rb") as stream:
        # Belgeyi akıştan yükleyin
        with Redactor(stream) as redactor:
            # Genel belge bilgilerini alın
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) tıklayın.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
