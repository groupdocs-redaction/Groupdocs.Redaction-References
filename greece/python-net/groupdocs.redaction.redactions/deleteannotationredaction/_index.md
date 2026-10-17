---
title: "Κλάση DeleteAnnotationRedaction"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια κειμενική απόκρυψη που διαγράφει τα σχόλια εάν το κείμενο ταιριάζει με μια δεδομένη κανονική έκφραση (προαιρετικά διαγράφει όλα τα σχόλια)."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

Αντιπροσωπεύει μια κειμενική απόκρυψη που διαγράφει τα σχόλια εάν το κείμενο ταιριάζει με μια δεδομένη κανονική έκφραση (προαιρετικά διαγράφει όλα τα σχόλια).

Μάθετε περισσότερα

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

Ο τύπος DeleteAnnotationRedaction εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης DeleteAnnotationRedaction, με ρυθμίσεις για διαγραφή όλων των σημειώσεων (που ταιριάζουν με όλα). |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης DeleteAnnotationRedaction, διαγράφοντας σημειώσεις που ταιριάζουν με την δοσμένη έκφραση. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης DeleteAnnotationRedaction, διαγράφοντας σημειώσεις που ταιριάζουν με την δοσμένη έκφραση. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | Εφαρμόζει τη redaction σε ένα δεδομένο αντικείμενο μορφής. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | Η περιγραφή της διαγραφής, που περιέχει το όνομα της διαγραφής και τις παραμέτρους. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | Η κανονική έκφραση για αντιστοίχιση. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # Διαγραφή σημειώσεων που περιέχουν τη λέξη "internal" (χωρίς διάκριση πεζών‑κεφαλαίων)
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν `DeleteAnnotationRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
