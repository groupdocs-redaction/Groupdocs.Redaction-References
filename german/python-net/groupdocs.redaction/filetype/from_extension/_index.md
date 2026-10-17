---
title: "from_extension Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Ordnet Dateierweiterungen dem Dateityp zu."
type: docs
url: /de/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

Ordnet Dateierweiterungen dem Dateityp zu.

```python
def from_extension(cls, extension):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| extension | `str` | Dateierweiterung (einschließlich des Punktes "."). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| Wirft | Beschreibung |
| :- | :- |
| `ValueError` | Wenn `extension` null oder ein leerer String ist. |

### Siehe auch
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
