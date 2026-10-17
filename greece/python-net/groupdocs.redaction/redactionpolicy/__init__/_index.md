---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο αντικείμενο RedactionPolicy."
type: docs
url: /el/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

Αρχικοποιεί ένα νέο αντικείμενο RedactionPolicy.

```python
def __init__(self):
    ...
```

### Παράδειγμα

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

Αρχικοποιεί ένα νέο RedactionPolicy με μια συγκεκριμένη λίστα διαγραφών.

```python
def __init__(self, redactions):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| redactions | `list[Redaction]` | Ένας πίνακας redactions για την πολιτική. |

### Παράδειγμα

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### Δείτε επίσης
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
