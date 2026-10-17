---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο αντικείμενο της κλάσης DeleteAnnotationRedaction, με ρυθμίσεις για διαγραφή όλων των σημειώσεων (που ταιριάζουν με όλα)."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης DeleteAnnotationRedaction, με ρυθμίσεις για διαγραφή όλων των σημειώσεων (που ταιριάζουν με όλα).

```python
def __init__(self):
    ...
```

### Παράδειγμα

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Διαγραφή όλων των σχολίων
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης DeleteAnnotationRedaction, διαγράφοντας σημειώσεις που ταιριάζουν με την δοσμένη έκφραση.

```python
def __init__(self, pattern):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| pattern | `str` | Κανονική έκφραση. |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Διαγραφή σημειώσεων που περιέχουν τη λέξη "internal" (χωρίς διάκριση πεζών‑κεφαλαίων)
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης DeleteAnnotationRedaction, διαγράφοντας σημειώσεις που ταιριάζουν με την δοσμένη έκφραση.

```python
def __init__(self, regex):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Κανονική έκφραση. |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Διαγραφή σχολίων των οποίων το περιεχόμενο ταιριάζει με τη regex (χωρίς διάκριση πεζών‑κεφαλαίων)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### Δείτε επίσης
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
