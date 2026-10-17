---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο αντικείμενο του RegexRedaction."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

Αρχικοποιεί ένα νέο αντικείμενο του RegexRedaction.

```python
def __init__(self, pattern, options):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| pattern | `str` | Κανονική έκφραση για αναζήτηση και αντικατάσταση. |
| options | `ReplacementOptions` | Επιλογές αντικατάστασης (κειμενικές, χρώμα). |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

Αρχικοποιεί ένα νέο αντικείμενο RegexRedaction.

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
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### Δείτε επίσης
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
