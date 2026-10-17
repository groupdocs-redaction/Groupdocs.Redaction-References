---
title: "get_supported_file_types metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Hämtar stödda filtyper."
type: docs
url: /sv/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

Hämtar stödda filtyper.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### Exempel

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Hämta samlingen av stödda filtyper
    supported_file_types = FileType.get_supported_file_types()

    # Enumerera filtyperna sorterade efter filändelse
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

### Se även
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
