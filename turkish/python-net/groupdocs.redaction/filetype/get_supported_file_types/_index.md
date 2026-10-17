---
title: "get_supported_file_types metodu"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Desteklenen dosya türlerini alır."
type: docs
url: /tr/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

Desteklenen dosya türlerini alır.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### Örnek

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

### Ayrıca Bakınız
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
