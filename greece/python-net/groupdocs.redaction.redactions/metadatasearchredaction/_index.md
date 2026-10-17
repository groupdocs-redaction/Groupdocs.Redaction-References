---
title: "κλάση MetadataSearchRedaction"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια επεξεργασία μεταδεδομένων που αναζητά και επεξεργάζεται μεταδεδομένα χρησιμοποιώντας κανονικές εκφράσεις, ταιριάζοντας κλειδιά και/ή τιμές."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

Αντιπροσωπεύει μια επεξεργασία μεταδεδομένων που αναζητά και επεξεργάζεται μεταδεδομένα χρησιμοποιώντας κανονικές εκφράσεις, ταιριάζοντας κλειδιά και/ή τιμές.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

Ο τύπος MetadataSearchRedaction εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας την τιμή για την αντιστοίχιση των καλυμμένων στοιχείων. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | Αρχικοποιεί μια νέα παρουσία του MetadataSearchRedaction, χρησιμοποιώντας το όνομα και την τιμή του στοιχείου για την αντιστοίχιση των καλυμμένων στοιχείων. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας την τιμή για την αντιστοίχιση των καλυμμένων στοιχείων. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | Αρχικοποιεί μια νέα παρουσία του MetadataSearchRedaction χρησιμοποιώντας το όνομα και την τιμή του στοιχείου για την αντιστοίχιση των καλυμμένων στοιχείων. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Εφαρμόζει τη διαγραφή σε μια δεδομένη παρουσία μορφής. (κληρονομείται από [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (κληρονομείται από [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | Η περιγραφή της redaction, που περιλαμβάνει το όνομα και τις παραμέτρους της. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | Η κανονική έκφραση για την αντιστοίχιση του ονόματος (κλειδιού) ενός μεταδεδομένου στοιχείου. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | Η τιμή κειμενικής αντικατάστασης. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | Η κανονική έκφραση για την αντιστοίχιση του κειμένου τιμής ενός μεταδεδομένου στοιχείου. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Το φίλτρο που χρησιμοποιείται για την επιλογή όλων ή συγκεκριμένων μεταδεδομένων, όπως Συγγραφέας ή Εταιρεία. (κληρονομείται από [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Καλύψτε οποιαδήποτε τιμή μεταδεδομένων που ταιριάζει με το μοτίβο
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν `MetadataSearchRedaction`:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
