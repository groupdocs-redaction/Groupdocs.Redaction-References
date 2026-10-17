---
title: "from_extension-methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Koppelt bestandsextensie aan bestandstype."
type: docs
url: /nl/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

Koppelt bestandsextensie aan bestandstype.

```python
def from_extension(cls, extension):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| extension | `str` | Bestandsextensie (inclusief de punt "."). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| Foutmeldingen | Beschrijving |
| :- | :- |
| `ValueError` | Wanneer `extension` null of een lege tekenreeks is. |

### Zie ook
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
