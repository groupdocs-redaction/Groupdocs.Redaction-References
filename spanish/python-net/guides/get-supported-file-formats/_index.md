---
title: "Obtener formatos de archivo compatibles"
linkTitle: "Get supported file formats"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Este artículo muestra cómo obtener la lista de todos los formatos de archivo compatibles de GroupDocs.Redaction usando Python."
type: docs
url: /es/python-net/guides/get-supported-file-formats/
is_root: false
weight: 130
---


GroupDocs.Redaction permite obtener la lista de todos los formatos de archivo compatibles mediante los siguientes pasos:

*   Call [GetSupportedFileTypes](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/get_supported_file_types/) of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) class;
*   Enumerate through the collection of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) objects*.*

El siguiente ejemplo muestra cómo obtener la lista de formatos de archivo compatibles.

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Recuperar la colección de tipos de archivo compatibles
    supported_file_types = FileType.get_supported_file_types()

    # Enumerar los tipos de archivo ordenados por extensión
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

  
```text
Bitmap Image File (.bmp)
Comma Separated Values File (.csv)
Microsoft Word Document (.doc)
Word Open XML Macro-Enabled Document (.docm)
Microsoft Word Open XML Document (.docx)
Word Document Template (.dot)
Word Open XML Macro-Enabled Document Template (.dotm)
Word Open XML Document Template (.dotx)
Graphical Interchange Format File (.gif)
Hypertext Markup Language File (.htm)
[TRUNCATED]
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-supported-file-formats/list_supported_formats/list-supported-formats.txt)
