---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο CellColumnRedaction."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

Αρχικοποιεί ένα νέο CellColumnRedaction.

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| filter | `CellFilter` | Φίλτρο στήλης και φύλλου εργασίας. |
| reg_ex | `System.Text.RegularExpressions.Regex` | Κανονική έκφραση για αναζήτηση και αντικατάσταση. |
| options | `ReplacementOptions` | Επιλογές αντικατάστασης. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("spreadsheet.xlsx") as redactor:
    redactor.apply(
        CellColumnRedaction(
            CellFilter(worksheet="Sheet1", column=2),
            r"\bsecret\b",
            ReplacementOptions(Color.BLACK)
        )
    )
    redactor.save()
```

### Δείτε επίσης
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
