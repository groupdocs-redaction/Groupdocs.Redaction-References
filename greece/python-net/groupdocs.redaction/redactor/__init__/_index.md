---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο αντικείμενο Redactor χρησιμοποιώντας διαδρομή αρχείου."
type: docs
url: /el/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

Αρχικοποιεί ένα νέο αντικείμενο Redactor χρησιμοποιώντας διαδρομή αρχείου.

```python
def __init__(self, file_path):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| file_path | `str` | Διαδρομή προς το αρχείο. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # Εκτελέστε εδώ τις λειτουργίες διαγραφής
    pass
```

## __init__ {#document}

Αρχικοποιεί ένα νέο αντικείμενο [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) χρησιμοποιώντας ροή.

```python
def __init__(self, document):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| document | `io.RawIOBase` | Ροή προέλευσης του εγγράφου. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # Ανοίξτε το έγγραφο ως δυαδική ροή
    with open("./sample.pdf", "rb") as stream:
        # Φορτώστε το έγγραφο από τη ροή
        with Redactor(stream) as redactor:
            # Εκτελέστε τις διαγραφές εδώ
            pass
```

## __init__ {#file_path-load_options}

Αρχικοποιεί ένα νέο αντικείμενο [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) για έγγραφο προστατευμένο με κωδικό χρησιμοποιώντας τη διαδρομή του.

```python
def __init__(self, file_path, load_options):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| file_path | `str` | Διαδρομή προς το αρχείο. |
| load_options | `LoadOptions` | Επιλογές, συμπεριλαμβανομένου κωδικού πρόσβασης. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor

# Φορτώστε ένα έγγραφο προστατευμένο με κωδικό πρόσβασης από διαδρομή αρχείου
with Redactor("protected.docx") as redactor:
    # Εκτελέστε εδώ τις λειτουργίες διαγραφής
    pass
```

## __init__ {#file_path-load_options-settings}

Αρχικοποιεί ένα νέο αντικείμενο Redactor για έγγραφο προστατευμένο με κωδικό χρησιμοποιώντας τη διαδρομή του και τις ρυθμίσεις.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| file_path | `str` | Διαδρομή προς το αρχείο. |
| load_options | `LoadOptions` | Επιλογές εξαρτημένες από το αρχείο, συμπεριλαμβανομένου κωδικού πρόσβασης. |
| settings | `RedactorSettings` | Προεπιλεγμένες ρυθμίσεις για τη διαδικασία διαγραφής. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

Αρχικοποιεί ένα νέο αντικείμενο Redactor για έγγραφο προστατευμένο με κωδικό χρησιμοποιώντας ροή.

```python
def __init__(self, document, load_options):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| document | `io.RawIOBase` | Ροή εισόδου προέλευσης. |
| load_options | `LoadOptions` | Επιλογές, συμπεριλαμβανομένου κωδικού πρόσβασης. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # Ανοίξτε το προστατευμένο PDF ως δυαδική ροή
    with open(r"C:\sample.pdf", "rb") as stream:
        # Παρέχετε τον κωδικό πρόσβασης μέσω LoadOptions
        load_options = LoadOptions("mypassword")
        # Αρχικοποιήστε το Redactor με τη ροή και τις επιλογές φόρτωσης
        with Redactor(stream, load_options) as redactor:
            # Εκτελέστε εδώ τις λειτουργίες διαγραφής
            pass
```

## __init__ {#document-load_options-settings}

Αρχικοποιεί ένα νέο αντικείμενο [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) για έγγραφο προστατευμένο με κωδικό χρησιμοποιώντας ροή και ρυθμίσεις.

```python
def __init__(self, document, load_options, settings):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| document | `io.RawIOBase` | Ροή εισόδου προέλευσης. |
| load_options | `LoadOptions` | Επιλογές, συμπεριλαμβανομένου κωδικού πρόσβασης. |
| settings | `RedactorSettings` | Προεπιλεγμένες ρυθμίσεις για τη διαδικασία επεξεργασίας. |

### Δείτε επίσης
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
