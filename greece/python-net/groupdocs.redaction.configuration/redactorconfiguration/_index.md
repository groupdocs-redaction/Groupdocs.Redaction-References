---
title: "RedactorConfiguration κλάση"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Παρέχει πρόσβαση σε μια λίστα υποστηριζόμενων μορφών, ενσωματωμένων και προσαρμοσμένων μορφών χρήστη."
type: docs
url: /el/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

Παρέχει πρόσβαση σε μια λίστα υποστηριζόμενων μορφών, ενσωματωμένων και προσαρμοσμένων μορφών χρήστη.

Μάθετε περισσότερα:

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Ο τύπος RedactorConfiguration εκθέτει τα παρακάτω μέλη:

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | Εντοπίζει τις ρυθμίσεις μορφής για μια δεδομένη επέκταση αρχείου. |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | Επιστρέφει ένα μοναδικό (singleton) αντικείμενο με την προεπιλεγμένη ρύθμιση των ενσωματωμένων μορφών. |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | Η λίστα των αναγνωρισμένων μορφών, δείτε [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### Παράδειγμα

```python
# Προσθέστε έναν προσαρμοσμένο χειριστή μορφής χρήστη
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# Ανακτήστε έναν ενσωματωμένο ή προσαρμοσμένο χειριστή μορφής χρήστη
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### Δείτε επίσης
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
