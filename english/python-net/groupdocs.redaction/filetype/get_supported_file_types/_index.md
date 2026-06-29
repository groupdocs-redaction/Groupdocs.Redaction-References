---
title: get_supported_file_types method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Retrieves supported file types."
type: docs
url: /python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

Retrieves supported file types.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### Example

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Retrieve the collection of supported file types
    supported_file_types = FileType.get_supported_file_types()

    # Enumerate the file types sorted by extension
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

### See Also
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
