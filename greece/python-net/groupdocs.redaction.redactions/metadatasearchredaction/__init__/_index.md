---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας την τιμή για την αντιστοίχιση των καλυμμένων στοιχείων."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας την τιμή για την αντιστοίχιση των καλυμμένων στοιχείων.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| value_pattern | `str` | Κανονική έκφραση για αναζήτηση και αντικατάσταση |
| replacement | `str` | Κειμενική αντικατάσταση |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

Αρχικοποιεί μια νέα παρουσία του MetadataSearchRedaction, χρησιμοποιώντας το όνομα και την τιμή του στοιχείου για την αντιστοίχιση των καλυμμένων στοιχείων.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| value_pattern | `str` | Κανονική έκφραση για αναζήτηση και αντικατάσταση τιμής στοιχείου μεταδεδομένων. |
| replacement | `str` | Κειμενική αντικατάσταση. |
| key_pattern | `str` | Κανονική έκφραση για αναζήτηση και αντικατάσταση ονόματος στοιχείου μεταδεδομένων. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # Αντικαταστήστε οποιαδήποτε διεύθυνση email που βρέθηκε στις τιμές μεταδεδομένων
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας την τιμή για την αντιστοίχιση των καλυμμένων στοιχείων.

```python
def __init__(self, value_regex, replacement):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Κανονική έκφραση για αναζήτηση και αντικατάσταση. |
| replacement | `str` | Κειμενική αντικατάσταση. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# Απόκρυψη οποιασδήποτε διεύθυνσης email στα μεταδεδομένα
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

Αρχικοποιεί μια νέα παρουσία του MetadataSearchRedaction χρησιμοποιώντας το όνομα και την τιμή του στοιχείου για την αντιστοίχιση των καλυμμένων στοιχείων.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Κανονική έκφραση για αναζήτηση και αντικατάσταση τιμής στοιχείου μεταδεδομένων. |
| replacement | `str` | Κειμενική αντικατάσταση. |
| key_regex | `System.Text.RegularExpressions.Regex` | Κανονική έκφραση για αναζήτηση και αντικατάσταση ονόματος στοιχείου μεταδεδομένων. |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# Απόκρυψη διευθύνσεων email στις τιμές μεταδεδομένων
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### Δείτε επίσης
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
