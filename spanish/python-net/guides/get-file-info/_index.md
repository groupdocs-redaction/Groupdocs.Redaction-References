---
title: "Obtener información del archivo"
linkTitle: "Get file info"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Este artículo explica la capacidad de la API de GroupDocs.Redaction para obtener la información general del documento, que incluye FileType, PageCount y FileSize."
type: docs
url: /es/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction proporciona información general del documento, que incluye:

*   FileType
*   PageCount
*   FileSize

Los siguientes ejemplos de código demuestran cómo obtener información del documento.

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # Cargar el documento desde el disco local
    with Redactor("./sample.docx") as redactor:
        # Recuperar información general del documento
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` es el archivo de ejemplo utilizado en este ejemplo. Haz clic en [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) para descargarlo.

  
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
    # Abrir el documento como un flujo binario
    with open("./sample.docx", "rb") as stream:
        # Cargar el documento desde el flujo
        with Redactor(stream) as redactor:
            # Recuperar información general del documento
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` es el archivo de ejemplo utilizado en este ejemplo. Haz clic en [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) para descargarlo.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
