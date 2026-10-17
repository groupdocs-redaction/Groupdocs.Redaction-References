---
title: "DocumentFormatConfiguration κλάση"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια αναφορά τύπου για κλάση που προέρχεται από DocumentFormatInstance και μια λίστα υποστηριζόμενων επεκτάσεων αρχείων για ταχύτερη ανίχνευση μορφής."
type: docs
url: /el/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

Αντιπροσωπεύει μια αναφορά τύπου για την κλάση που προέρχεται από το [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) και μια λίστα υποστηριζόμενων επεκτάσεων αρχείων για ταχύτερη ανίχνευση μορφής.

Μάθετε περισσότερα

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Ο τύπος DocumentFormatConfiguration εκθέτει τα παρακάτω μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | Αρχικοποιεί ένα νέο αντικείμενο DocumentFormatConfiguration. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | Ελέγχει αν μια δεδομένη επέκταση αρχείου μπορεί να αντιμετωπιστεί ως DocumentType. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | Ο τύπος μιας κλάσης που κληρονομεί από [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | Η λίστα επεκτάσεων αρχείων χωρισμένη με κόμμα (π.χ. \".pdf\"), χωρίς διάκριση πεζών‑κεφαλαίων. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | Τα δεδομένα που απαιτούνται για την αρχικοποίηση του [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |

### Παράδειγμα

```python
from groupdocs.redaction import DocumentFormatConfiguration

# Δημιουργήστε μια προσαρμοσμένη διαμόρφωση μορφής
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### Δείτε επίσης
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
