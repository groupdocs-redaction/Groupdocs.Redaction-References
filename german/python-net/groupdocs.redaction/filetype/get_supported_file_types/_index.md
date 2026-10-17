---
title: "get_supported_file_types Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Ruft unterstützte Dateitypen ab."
type: docs
url: /de/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

Ruft unterstützte Dateitypen ab.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### Beispiel

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Rufen Sie die Sammlung unterstützter Dateitypen ab
    supported_file_types = FileType.get_supported_file_types()

    # Durchlaufen Sie die Dateitypen, sortiert nach Erweiterung
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

### Siehe auch
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
