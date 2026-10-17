---
title: "méthode get_supported_file_types"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Récupère les types de fichiers pris en charge."
type: docs
url: /fr/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

Récupère les types de fichiers pris en charge.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### Exemple

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Récupérer la collection des types de fichiers pris en charge
    supported_file_types = FileType.get_supported_file_types()

    # Énumérer les types de fichiers triés par extension
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

### Voir aussi
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
