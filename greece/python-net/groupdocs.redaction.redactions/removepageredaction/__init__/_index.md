---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο RemovePageRedaction."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

Αρχικοποιεί ένα νέο RemovePageRedaction.

```python
def __init__(self, origin, index, count):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Αναζήτηση θέσης αναφοράς, την αρχή ή το τέλος ενός εγγράφου. |
| index | `int` | Δείκτης αρχικής θέσης (από 0). |
| count | `int` | Αριθμός σελίδων προς αφαίρεση. |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Αφαιρέστε 3 σελίδες ξεκινώντας από τη δεύτερη σελίδα (δείκτης 0‑βασισμένο 1)
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### Δείτε επίσης
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
