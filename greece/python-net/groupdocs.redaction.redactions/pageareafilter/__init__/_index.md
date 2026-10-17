---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο PageAreaFilter για τη διαγραφή μιας συγκεκριμένης περιοχής."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

Αρχικοποιεί ένα νέο PageAreaFilter για τη διαγραφή μιας συγκεκριμένης περιοχής.

```python
def __init__(self, top_left, size):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Συντεταγμένες περιοχής επάνω‑αριστερά. |
| size | `System.Drawing.Size` | Μέγεθος περιοχής και χρώμα. |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### Δείτε επίσης
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
