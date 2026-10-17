---
title: "Κλάση Redactor"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει την κύρια κλάση που ελέγχει τη διαδικασία επεξεργασίας εγγράφων, επιτρέποντας το άνοιγμα, την επεξεργασία και την αποθήκευση εγγράφων."
type: docs
url: /el/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

Αντιπροσωπεύει την κύρια κλάση που ελέγχει τη διαδικασία επεξεργασίας εγγράφων, επιτρέποντας το άνοιγμα, την επεξεργασία και την αποθήκευση εγγράφων.

Μάθετε περισσότερα
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

Ο τύπος Redactor εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | Αρχικοποιεί ένα νέο αντικείμενο Redactor χρησιμοποιώντας διαδρομή αρχείου. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | Αρχικοποιεί ένα νέο αντικείμενο [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) χρησιμοποιώντας ροή. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | Αρχικοποιεί ένα νέο αντικείμενο [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) για έγγραφο προστατευμένο με κωδικό χρησιμοποιώντας τη διαδρομή του. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | Αρχικοποιεί ένα νέο αντικείμενο Redactor για έγγραφο προστατευμένο με κωδικό χρησιμοποιώντας τη διαδρομή του και τις ρυθμίσεις. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | Αρχικοποιεί ένα νέο αντικείμενο Redactor για έγγραφο προστατευμένο με κωδικό χρησιμοποιώντας ροή. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | Αρχικοποιεί ένα νέο αντικείμενο [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) για έγγραφο προστατευμένο με κωδικό χρησιμοποιώντας ροή και ρυθμίσεις. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | Εφαρμόζει μια επεμβαση στο έγγραφο. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | Εφαρμόζει ένα σύνολο επεμβάσεων στο έγγραφο. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | Εφαρμόζει μια πολιτική επεμβάσεων στο έγγραφο. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | Απελευθερώνει πόρους. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | Δημιουργεί εικόνες προεπισκόπησης συγκεκριμένων σελίδων σε δεδομένη μορφή εικόνας. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | Ανακτά τις γενικές πληροφορίες για το έγγραφο, όπως το μέγεθος και τον αριθμό σελίδων. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | Αποθηκεύει το έγγραφο σε αρχείο με τις ακόλουθες επιλογές: AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | Αποθηκεύει το έγγραφο σε αρχείο. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | Αποθηκεύει το έγγραφο σε ροή, συμπεριλαμβανομένης της προσαρμοσμένης τοποθεσίας. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Ανοίξτε ένα έγγραφο και αφαιρέστε την πρώτη σελίδα
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν `Redactor`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### Δείτε επίσης
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
