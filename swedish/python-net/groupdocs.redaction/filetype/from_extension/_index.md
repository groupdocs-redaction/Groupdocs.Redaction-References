---
title: "from_extension‑metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Kopplar filändelse till filtyp."
type: docs
url: /sv/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

Kopplar filändelse till filtyp.

```python
def from_extension(cls, extension):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| extension | `str` | Filändelse (inklusive punkten "."). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| Uppstår | Beskrivning |
| :- | :- |
| `ValueError` | När `extension` är null eller en tom sträng. |

### Se även
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
