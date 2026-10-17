---
title: "Κλάση RedactorSettings"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει τις ρυθμίσεις επεμβάσεων, επιτρέποντας την προσαρμογή της διαδικασίας επεξεργασίας."
type: docs
url: /el/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

Αντιπροσωπεύει τις ρυθμίσεις επεμβάσεων, επιτρέποντας την προσαρμογή της διαδικασίας επεξεργασίας.

Μάθετε περισσότερα

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

Ο τύπος RedactorSettings εκθέτει τα παρακάτω μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | Αρχικοποιεί ένα νέο αντίτυπο της κλάσης RedactorSettings. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | Αρχικοποιεί ένα νέο αντίτυπο RedactorSettings με ένα δεδομένο αντίτυπο ILogger. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | Αρχικοποιεί ένα νέο αντίτυπο της κλάσης RedactorSettings με ένα δεδομένο αντίτυπο IRedactionCallback. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | Αρχικοποιεί ένα νέο αντίτυπο RedactorSettings με το καθορισμένο IOcrConnector. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | Αρχικοποιεί ένα νέο αντίτυπο RedactorSettings με τον καθορισμένο καταγραφέα και το callback. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | Αρχικοποιεί ένα νέο αντίτυπο της κλάσης RedactorSettings με δεδομένα αντίτυπα ILogger, IRedactionCallback και IOcrConnector. |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | Ο καταγραφέας που χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων. Πρέπει να είναι ένα αντίτυπο κλάσης που υλοποιεί [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/). |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | Το αντίτυπο του συνδέσμου OCR που υλοποιεί [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/). |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | Η κλήση επιστροφής απόσυρσης που χρησιμοποιείται για την αξιολόγηση κάθε περιγραφής απόσυρσης. |

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

### Δείτε επίσης
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
