---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο αντικείμενο PageAreaRedaction."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

Αρχικοποιεί ένα νέο αντικείμενο PageAreaRedaction.

```python
def __init__(self, regex, options):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Κανονική έκφραση για αναζήτηση και αντικατάσταση. |
| options | `ReplacementOptions` | Επιλογές αντικατάστασης (κειμενικές, χρώμα). |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(r"\d{3}-\d{2}-\d{4}", ReplacementOptions("[SSN]"))
    )
    redactor.save()
```

## __init__ {#regex-options-image_options}

Αρχικοποιεί ένα νέο PageAreaRedaction.

```python
def __init__(self, regex, options, image_options):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Κανονική έκφραση για αναζήτηση και αντικατάσταση. |
| options | `ReplacementOptions` | Επιλογές αντικατάστασης (κειμενικές, χρώμα). |
| image_options | `RegionReplacementOptions` | Επιλογές αντικατάστασης (περιοχή εικόνας). |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

redactor = Redactor("scan.pdf")
redactor.apply(
    PageAreaRedaction(
        r"\d{3}-\d{2}-\d{4}",
        ReplacementOptions("[SSN]"),
        RegionReplacementOptions(Color.BLACK, Size(120, 20))
    )
)
redactor.save()
```

### Δείτε επίσης
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
