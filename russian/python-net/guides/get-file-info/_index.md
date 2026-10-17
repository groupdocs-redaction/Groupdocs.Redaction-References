---
title: "Получить информацию о файле"
linkTitle: "Get file info"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "В этой статье объясняется возможность API GroupDocs.Redaction получать общую информацию о документе, которая включает тип файла (FileType), количество страниц (PageCount) и размер файла (FileSize)."
type: docs
url: /ru/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction предоставляет общую информацию о документе, которая включает:

*   FileType
*   PageCount
*   FileSize

Следующие примеры кода демонстрируют, как получить информацию о документе.

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # Загрузите документ с локального диска
    with Redactor("./sample.docx") as redactor:
        # Получите общую информацию о документе
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx), чтобы скачать его.

  
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
    # Откройте документ как бинарный поток
    with open("./sample.docx", "rb") as stream:
        # Загрузите документ из потока
        with Redactor(stream) as redactor:
            # Получите общую информацию о документе
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx), чтобы скачать его.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
