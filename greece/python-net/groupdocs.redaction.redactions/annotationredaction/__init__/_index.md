---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο AnnotationRedaction με ένα πρότυπο regex και κείμενο αντικατάστασης."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

Αρχικοποιεί ένα νέο AnnotationRedaction με ένα πρότυπο regex και κείμενο αντικατάστασης.

```python
def __init__(self, pattern, replacement):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| pattern | `str` | Κανονική έκφραση για αντιστοίχιση. |
| replacement | `str` | Κειμενική αντικατάσταση για το ταιριασμένο κείμενο. |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Απόκρυψη της λέξης "approved" στα κείμενα σχολίων
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

Αρχικοποιεί ένα νέο παράδειγμα του [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/).

```python
def __init__(self, regex, replacement):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Κανονική έκφραση για αντιστοίχιση. |
| replacement | `str` | Κειμενική αντικατάσταση για το ταιριασμένο κείμενο. |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Απόκρυψη της λέξης "approved" (χωρίς διάκριση πεζών‑κεφαλαίων) και αντικατάστασή της με "[REVIEW]"
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### Δείτε επίσης
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
