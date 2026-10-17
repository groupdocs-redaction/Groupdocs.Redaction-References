---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο ImageAreaRedaction για τη διαγραφή μιας συγκεκριμένης ορθογώνιας περιοχής."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

Αρχικοποιεί ένα νέο ImageAreaRedaction για τη διαγραφή μιας συγκεκριμένης ορθογώνιας περιοχής.

```python
def __init__(self, top_left, options):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Συντεταγμένες περιοχής επάνω‑αριστερά. |
| options | `RegionReplacementOptions` | Μέγεθος περιοχής και χρώμα. |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# Ορίστε την πάνω‑αριστερή γωνία της περιοχής που θα αποκρυφθεί
top_left = Point(385, 485)
# Ορίστε το μέγεθος και το χρώμα της περιοχής απόκρυψης
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# Δημιουργήστε το αντικείμενο απόκρυψης
redaction = ImageAreaRedaction(top_left, region_options)
```

### Δείτε επίσης
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
