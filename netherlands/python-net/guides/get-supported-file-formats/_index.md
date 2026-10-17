---
title: "Ophalen ondersteunde bestandsformaten"
linkTitle: "Get supported file formats"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Dit artikel laat zien hoe u de lijst met alle ondersteunde bestandsformaten van GroupDocs.Redaction kunt verkrijgen met Python."
type: docs
url: /nl/python-net/guides/get-supported-file-formats/
is_root: false
weight: 130
---


GroupDocs.Redaction maakt het mogelijk om de lijst met alle ondersteunde bestandsformaten te verkrijgen via de volgende stappen:

*   Call [GetSupportedFileTypes](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/get_supported_file_types/) of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) class;
*   Enumerate through the collection of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) objects*.*

Het volgende voorbeeld laat zien hoe u de lijst met ondersteunde bestandsformaten kunt ophalen.

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Haal de collectie van ondersteunde bestandstypen op
    supported_file_types = FileType.get_supported_file_types()

    # Som de bestandstypen op gesorteerd op extensie
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
