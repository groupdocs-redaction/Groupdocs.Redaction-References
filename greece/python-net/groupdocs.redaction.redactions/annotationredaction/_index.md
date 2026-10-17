---
title: "Κλάση AnnotationRedaction"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια απόκρυψη που αντικαθιστά το κείμενο σχολίων (σχόλια κ.λπ.) που ταιριάζει με μια δεδομένη κανονική έκφραση."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

Αντιπροσωπεύει μια απόκρυψη που αντικαθιστά το κείμενο σχολίων (σχόλια κ.λπ.) που ταιριάζει με μια δεδομένη κανονική έκφραση.

Μάθετε περισσότερα

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

Ο τύπος AnnotationRedaction εκθέτει τα παρακάτω μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | Αρχικοποιεί ένα νέο AnnotationRedaction με ένα πρότυπο regex και κείμενο αντικατάστασης. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | Αρχικοποιεί ένα νέο παράδειγμα του [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/). |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | Εφαρμόζει τη redaction σε ένα δεδομένο αντικείμενο μορφής. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | Η περιγραφή της διαγραφής, περιγράφοντας τη διαγραφή και τις παραμέτρους της. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | Η κανονική έκφραση για αντιστοίχιση. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | Η κειμενική αντικατάσταση για το ταιριασμένο κείμενο. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν `AnnotationRedaction`:

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
