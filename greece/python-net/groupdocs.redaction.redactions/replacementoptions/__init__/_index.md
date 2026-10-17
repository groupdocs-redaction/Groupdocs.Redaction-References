---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο αντικείμενο του ReplacementOptions με το καθορισμένο κείμενο αντικατάστασης."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

Αρχικοποιεί ένα νέο αντικείμενο του ReplacementOptions με το καθορισμένο κείμενο αντικατάστασης.

```python
def __init__(self, replacement):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| replacement | `str` | Κειμενική αντικατάσταση. |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Αντικατάσταση ταιριακού κειμένου με "[REDACTED]"
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ReplacementOptions με χρωματιστό ορθογώνιο ως επιλογή.

```python
def __init__(self, color):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| color | `System.Drawing.Color` | Χρώμα ορθογωνίου. |

### Δείτε επίσης
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
