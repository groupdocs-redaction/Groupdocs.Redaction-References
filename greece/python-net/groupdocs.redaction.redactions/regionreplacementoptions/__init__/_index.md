---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο αντικείμενο RegionReplacementOptions."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

Αρχικοποιεί ένα νέο αντικείμενο RegionReplacementOptions.

```python
def __init__(self, fill_color, size):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Χρώμα για τη γέμιση της περιοχής. |
| size | `System.Drawing.Size` | Μέγεθος γεμισμένης περιοχής. |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RegionReplacementOptions του οποίου το μέγεθος ταιριάζει με το δεδομένο κείμενο.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Χρώμα για τη γέμιση της περιοχής. |
| font | `System.Drawing.Font` | Αναμενόμενη γραμματοσειρά κειμένου. |
| expected_text | `str` | Αναμενόμενο κείμενο. |

### Δείτε επίσης
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
