---
title: "load μέθοδος"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Φορτώνει ένα RedactionPolicy από αρχείο XML."
type: docs
url: /el/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

Φορτώνει ένα RedactionPolicy από αρχείο XML.

```python
def load(cls, file_path):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| file_path | `str` | Διαδρομή προς το αρχείο XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Παράδειγμα

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

Φορτώνει ένα αντικείμενο RedactionPolicy από ροή που περιέχει διαμόρφωση XML.

```python
def load(cls, input):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| input | `io.RawIOBase` | Ροή που περιέχει τη διαμόρφωση XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Παράδειγμα

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# Φόρτωση της πολιτικής από αρχείο XML
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# Εφαρμόστε την πολιτική σε ένα έγγραφο
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Δείτε επίσης
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
