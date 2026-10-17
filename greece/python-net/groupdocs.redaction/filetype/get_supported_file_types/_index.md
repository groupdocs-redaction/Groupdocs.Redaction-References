---
title: "get_supported_file_types μέθοδος"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Ανακτά τους υποστηριζόμενους τύπους αρχείων."
type: docs
url: /el/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

Ανακτά τους υποστηριζόμενους τύπους αρχείων.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### Παράδειγμα

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Ανακτήστε τη συλλογή των υποστηριζόμενων τύπων αρχείων
    supported_file_types = FileType.get_supported_file_types()

    # Απαριθμήστε τους τύπους αρχείων ταξινομημένους κατά επέκταση
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

### Δείτε επίσης
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
