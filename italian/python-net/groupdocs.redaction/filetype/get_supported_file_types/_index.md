---
title: "metodo get_supported_file_types"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Recupera i tipi di file supportati."
type: docs
url: /it/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

Recupera i tipi di file supportati.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### Esempio

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Recupera la collezione dei tipi di file supportati
    supported_file_types = FileType.get_supported_file_types()

    # Elenca i tipi di file ordinati per estensione
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

### Vedi anche
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
