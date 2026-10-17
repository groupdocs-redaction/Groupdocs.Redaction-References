---
title: "Bu makale, Python kullanarak GroupDocs.Redaction'ın desteklediği tüm dosya formatlarının listesini nasıl alacağınızı gösterir."
linkTitle: "Get supported file formats"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "GroupDocs.Redaction, aşağıdaki adımlarla tüm desteklenen dosya formatlarının listesini almanıza olanak tanır:"
type: docs
url: /tr/python-net/guides/get-supported-file-formats/
is_root: false
weight: 130
---


Aşağıdaki örnek, desteklenen dosya formatları listesinin nasıl alınacağını gösterir.

*   Call [GetSupportedFileTypes](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/get_supported_file_types/) of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) class;
*   Enumerate through the collection of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) objects*.*

Desteklenen dosya türleri koleksiyonunu alın

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Dosya türlerini uzantıya göre sıralayarak listeleyin
    supported_file_types = FileType.get_supported_file_types()

    # Redaksiyon temelleri
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
