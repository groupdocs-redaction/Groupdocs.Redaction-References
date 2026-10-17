---
title: "احصل على صيغ الملفات المدعومة"
linkTitle: "Get supported file formats"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "توضح هذه المقالة كيفية الحصول على قائمة بجميع صيغ الملفات المدعومة في GroupDocs.Redaction باستخدام بايثون."
type: docs
url: /ar/python-net/guides/get-supported-file-formats/
is_root: false
weight: 130
---


يتيح GroupDocs.Redaction الحصول على قائمة بجميع صيغ الملفات المدعومة عبر الخطوات التالية:

*   Call [GetSupportedFileTypes](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/get_supported_file_types/) of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) class;
*   Enumerate through the collection of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) objects*.*

المثال التالي يوضح كيفية الحصول على قائمة صيغ الملفات المدعومة.

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # استرجاع مجموعة أنواع الملفات المدعومة
    supported_file_types = FileType.get_supported_file_types()

    # عدد أنواع الملفات مرتبة حسب الامتداد
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
