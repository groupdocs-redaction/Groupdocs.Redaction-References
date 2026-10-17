---
title: "Unterstützte Dateiformate abrufen"
linkTitle: "Get supported file formats"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Dieser Artikel zeigt, wie man die Liste aller unterstützten Dateiformate von **GroupDocs.Redaction** mit Python erhält."
type: docs
url: /de/python-net/guides/get-supported-file-formats/
is_root: false
weight: 130
---


**GroupDocs.Redaction** ermöglicht das Abrufen der Liste aller unterstützten Dateiformate in folgenden Schritten:

*   Call [GetSupportedFileTypes](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/get_supported_file_types/) of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) class;
*   Enumerate through the collection of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) objects*.*

Das folgende Beispiel zeigt, wie man die Liste unterstützter Dateiformate abruft.

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Rufen Sie die Sammlung unterstützter Dateitypen ab
    supported_file_types = FileType.get_supported_file_types()

    # Durchlaufen Sie die Dateitypen, sortiert nach Erweiterung
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
