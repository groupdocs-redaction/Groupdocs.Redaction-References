---
title: "Obtenir les formats de fichiers pris en charge"
linkTitle: "Get supported file formats"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Cet article montre comment obtenir la liste de tous les formats de fichiers pris en charge par GroupDocs.Redaction en utilisant Python."
type: docs
url: /fr/python-net/guides/get-supported-file-formats/
is_root: false
weight: 130
---


GroupDocs.Redaction permet d’obtenir la liste de tous les formats de fichiers pris en charge en suivant ces étapes :

*   Call [GetSupportedFileTypes](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/get_supported_file_types/) of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) class;
*   Enumerate through the collection of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) objects*.*

L’exemple suivant montre comment obtenir la liste des formats de fichiers pris en charge.

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Récupérer la collection des types de fichiers pris en charge
    supported_file_types = FileType.get_supported_file_types()

    # Énumérer les types de fichiers triés par extension
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
