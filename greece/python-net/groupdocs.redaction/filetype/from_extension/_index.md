---
title: "μέθοδος from_extension"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιστοιχίζει την επέκταση αρχείου στον τύπο αρχείου."
type: docs
url: /el/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

Αντιστοιχίζει την επέκταση αρχείου στον τύπο αρχείου.

```python
def from_extension(cls, extension):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| extension | `str` | Επέκταση αρχείου (συμπεριλαμβανομένου του σημείου "."). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| Αναφέρει | Περιγραφή |
| :- | :- |
| `ValueError` | Όταν το `extension` είναι null ή κενή συμβολοσειρά. |

### Δείτε επίσης
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
