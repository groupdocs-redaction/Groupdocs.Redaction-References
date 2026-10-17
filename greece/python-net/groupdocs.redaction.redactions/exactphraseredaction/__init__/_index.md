---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο αντίγραφο του ExactPhraseRedaction σε λειτουργία χωρίς διάκριση πεζών‑κεφαλαίων."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

Αρχικοποιεί ένα νέο αντίγραφο του ExactPhraseRedaction σε λειτουργία χωρίς διάκριση πεζών‑κεφαλαίων.

```python
def __init__(self, search_phrase, options):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| search_phrase | `str` | Συμβολοσειρά για αναζήτηση και αντικατάσταση. |
| options | `ReplacementOptions` | Επιλογές αντικατάστασης (κειμενικές, χρώμα). |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Αντικαταστήστε τις εμφανίσεις του "John Doe" με "[CUSTOMER]" (χωρίς διάκριση πεζών-κεφαλαίων)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

Αρχικοποιεί ένα νέο αντίγραφο ExactPhraseRedaction.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| search_phrase | `str` | Συμβολοσειρά για αναζήτηση και αντικατάσταση. |
| is_case_sensitive | `bool` | Αληθές εάν απαιτείται αναζήτηση με διάκριση πεζών-κεφαλαίων. |
| options | `ReplacementOptions` | Επιλογές αντικατάστασης (κειμενικές, χρώμα). |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Απόκρυψη ακριβούς φράσης χωρίς διάκριση πεζών-κεφαλαίων
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# Απόκρυψη ακριβούς φράσης με διάκριση πεζών-κεφαλαίων
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### Δείτε επίσης
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
