---
title: "Κλάση PreviewOptions"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Παρέχει επιλογές για τον καθορισμό απαιτήσεων και αντιπροσώπων ροής για τη δημιουργία προεπισκόπησης."
type: docs
url: /el/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

Παρέχει επιλογές για τον καθορισμό απαιτήσεων και αντιπροσώπων ροής για τη δημιουργία προεπισκόπησης.

Η κλάση επιτρέπει τον καθορισμό της μορφής προεπισκόπησης, των διαστάσεων της εικόνας, των αριθμών σελίδων, και των αντιπροσώπων που δημιουργούν και προαιρετικά απελευθερώνουν ροές για κάθε παραγόμενη σελίδα.

Ο τύπος PreviewOptions εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | Αρχικοποιεί ένα νέο αντικείμενο PreviewOptions. Η ροή εξόδου θα κλείσει μετά τη χρήση. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | Αρχικοποιεί ένα νέο αντικείμενο PreviewOptions, προκαλώντας την επιστροφή της ροής εξόδου στον πελάτη για περαιτέρω χρήση. |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | Ο delegate δημιουργίας ροής σελίδας. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | Το ύψος προεπισκόπησης σελίδας. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | Οι αριθμοί σελίδων για τη δημιουργία προεπισκόπησης. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | Η μορφή εικόνας προεπισκόπησης. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | Ο delegate ολοκλήρωσης προεπισκόπησης σελίδας. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | Το πλάτος προεπισκόπησης σελίδας. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # Δημιουργήστε ένα αρχείο για την εικόνα προεπισκόπησης της συγκεκριμένης σελίδας
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")  # returns a writable binary stream

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### Δείτε επίσης
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
