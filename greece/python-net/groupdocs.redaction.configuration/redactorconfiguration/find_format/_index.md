---
title: "Μέθοδος find_format"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Εντοπίζει τις ρυθμίσεις μορφής για μια δεδομένη επέκταση αρχείου."
type: docs
url: /el/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

Εντοπίζει τις ρυθμίσεις μορφής για μια δεδομένη επέκταση αρχείου.

```python
def find_format(self, file_extension):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| file_extension | `str` | Επέκταση αρχείου, η μορφή είναι \".ext\". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### Παράδειγμα

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Αποκτήστε το singleton αντικείμενο διαμόρφωσης
config = RedactorConfiguration.get_instance()

# Ανακτήστε τις ρυθμίσεις μορφής για μια δεδομένη επέκταση
settings = config.find_format(".txt")
if settings:
    # Επεκτείνετε τη λίστα των υποστηριζόμενων επεκτάσεων, π.χ., προσθέστε .dump
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### Δείτε επίσης
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
