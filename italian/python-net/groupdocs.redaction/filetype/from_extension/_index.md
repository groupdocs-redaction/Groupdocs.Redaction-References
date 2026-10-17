---
title: "metodo from_extension"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Mappa l'estensione del file al tipo di file."
type: docs
url: /it/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

Mappa l'estensione del file al tipo di file.

```python
def from_extension(cls, extension):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| extension | `str` | Estensione file (incluso il punto "."). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| Genera | Descrizione |
| :- | :- |
| `ValueError` | Quando `extension` è null o una stringa vuota. |

### Vedi anche
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
