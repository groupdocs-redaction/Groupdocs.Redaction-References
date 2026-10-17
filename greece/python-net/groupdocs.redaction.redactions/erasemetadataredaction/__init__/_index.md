---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο παράδειγμα της κλάσης EraseMetadataRedaction, διαγράφοντας όλα τα μεταδεδομένα."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

Αρχικοποιεί ένα νέο παράδειγμα της κλάσης EraseMetadataRedaction, διαγράφοντας όλα τα μεταδεδομένα.

```python
def __init__(self):
    ...
```

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

Αρχικοποιεί μια νέα παρουσία της EraseMetadataRedaction, διαγράφοντας τα μεταδεδομένα που ταιριάζουν με τα καθορισμένα `MetadataFilters`.

```python
def __init__(self, filter):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| filter | `MetadataFilters` | Φίλτρο για μεταδεδομένα προς διαγραφή. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Διαγραφή όλων των μεταδεδομένων
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Διαγραφή μόνο του πεδίου μεταδεδομένων συγγραφέα
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Δείτε επίσης
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
