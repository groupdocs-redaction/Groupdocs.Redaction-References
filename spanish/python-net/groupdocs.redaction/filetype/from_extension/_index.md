---
title: "método from_extension"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Mapea la extensión de archivo al tipo de archivo."
type: docs
url: /es/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

Mapea la extensión de archivo al tipo de archivo.

```python
def from_extension(cls, extension):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| extension | `str` | Extensión de archivo (incluyendo el punto "."). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| Lanza | Descripción |
| :- | :- |
| `ValueError` | Cuando `extension` es nulo o una cadena vacía. |

### Ver también
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
