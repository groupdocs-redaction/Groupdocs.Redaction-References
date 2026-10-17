---
title: "get_supported_file_types methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Haalt ondersteunde bestandstypen op."
type: docs
url: /nl/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

Haalt ondersteunde bestandstypen op.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### Voorbeeld

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

### Zie ook
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
