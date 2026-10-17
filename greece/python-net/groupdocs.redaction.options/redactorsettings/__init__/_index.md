---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο αντίτυπο της κλάσης RedactorSettings."
type: docs
url: /el/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

Αρχικοποιεί ένα νέο αντίτυπο της κλάσης RedactorSettings.

```python
def __init__(self):
    ...
```

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

## __init__ {#logger}

Αρχικοποιεί ένα νέο αντίτυπο RedactorSettings με ένα δεδομένο αντίτυπο ILogger.

```python
def __init__(self, logger):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| logger | `ILogger` | Μία παρουσία κλάσης που υλοποιεί τη διεπαφή `ILogger`. |

## __init__ {#callback}

Αρχικοποιεί ένα νέο αντίτυπο της κλάσης RedactorSettings με ένα δεδομένο αντίτυπο IRedactionCallback.

```python
def __init__(self, callback):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| callback | `IRedactionCallback` | Μία παρουσία κλάσης που υλοποιεί τη διεπαφή IRedactionCallback. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import LoadOptions, RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", LoadOptions(), RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

## __init__ {#ocr_connector}

Αρχικοποιεί ένα νέο αντίτυπο RedactorSettings με το καθορισμένο IOcrConnector.

```python
def __init__(self, ocr_connector):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | Μία έγκυρη υλοποίηση της διεπαφής IOcrConnector. |

## __init__ {#logger-callback}

Αρχικοποιεί ένα νέο αντίτυπο RedactorSettings με τον καθορισμένο καταγραφέα και το callback.

```python
def __init__(self, logger, callback):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| logger | `ILogger` | Μία παρουσία κλάσης που υλοποιεί τη διεπαφή ILogger. |
| callback | `IRedactionCallback` | Μία παρουσία μιας κλάσης που υλοποιεί τη διεπαφή IRedactionCallback. |

### Παράδειγμα

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

Αρχικοποιεί ένα νέο αντίτυπο της κλάσης RedactorSettings με δεδομένα αντίτυπα ILogger, IRedactionCallback και IOcrConnector.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| logger | `ILogger` | Μία παρουσία μιας κλάσης που υλοποιεί τη διεπαφή `ILogger`. |
| callback | `IRedactionCallback` | Μία παρουσία μιας κλάσης που υλοποιεί τη διεπαφή `IRedactionCallback`. |
| ocr_connector | `IOcrConnector` | Μία παρουσία υλοποίησης της διεπαφής `IOcrConnector`. Μπορεί να είναι `None`. |

### Παράδειγμα

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### Δείτε επίσης
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
