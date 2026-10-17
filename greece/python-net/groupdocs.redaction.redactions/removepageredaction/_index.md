---
title: "Κλάση RemovePageRedaction"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια επεξεργασία που αφαιρεί μια σελίδα (διαφάνεια, φύλλο εργασίας κ.λπ.) από ένα έγγραφο."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

Αντιπροσωπεύει μια επεξεργασία που αφαιρεί μια σελίδα (διαφάνεια, φύλλο εργασίας κ.λπ.) από ένα έγγραφο.

Μάθετε περισσότερα
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

Ο τύπος RemovePageRedaction εκθέτει τα παρακάτω μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | Αρχικοποιεί ένα νέο RemovePageRedaction. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | Εφαρμόζει τη redaction σε ένα δεδομένο αντικείμενο μορφής. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | Ο αριθμός των σελίδων προς αφαίρεση. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | Ο δείκτης θέσης εκκίνησης (βάση 0). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | Η θέση αναφοράς αναζήτησης, είτε η αρχή είτε το τέλος ενός εγγράφου. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | Η περιγραφή της διαγραφής, που περιέχει το όνομά της και τις παραμέτρους. (κληρονομείται από [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Αφαίρεση 1 σελίδας, μετρώντας από το τέλος του εγγράφου
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(rem_opt)

        # Αποθηκεύστε το διαγραμμένο έγγραφο
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν `RemovePageRedaction`:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
