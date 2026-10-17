---
title: "méthode from_extension"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Mappe l'extension de fichier au type de fichier."
type: docs
url: /fr/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

Mappe l'extension de fichier au type de fichier.

```python
def from_extension(cls, extension):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| extension | `str` | Extension de fichier (y compris le point "."). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| Lève | Description |
| :- | :- |
| `ValueError` | Lorsque `extension` est nul ou une chaîne vide. |

### Voir aussi
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
