---
title: "طريقة get_supported_file_types"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يسترجع أنواع الملفات المدعومة."
type: docs
url: /ar/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

يسترجع أنواع الملفات المدعومة.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### مثال

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

### انظر أيضًا
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
