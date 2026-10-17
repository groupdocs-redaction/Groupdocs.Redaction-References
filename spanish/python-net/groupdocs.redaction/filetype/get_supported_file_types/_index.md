---
title: "método get_supported_file_types"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Recupera los tipos de archivo compatibles."
type: docs
url: /es/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

Recupera los tipos de archivo compatibles.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### Ejemplo

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Recuperar la colección de tipos de archivo compatibles
    supported_file_types = FileType.get_supported_file_types()

    # Enumerar los tipos de archivo ordenados por extensión
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

### Ver también
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
