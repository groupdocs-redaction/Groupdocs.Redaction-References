---
title: "Κλάση PageAreaFilter"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει φίλτρο επεξεργασίας, ορίζοντας μια περιοχή μέσα σε μια σελίδα εγγράφου για την εφαρμογή της επεξεργασίας."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

Αντιπροσωπεύει φίλτρο επεξεργασίας, ορίζοντας μια περιοχή μέσα σε μια σελίδα εγγράφου για την εφαρμογή της επεξεργασίας.

Μάθετε περισσότερα

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Ο τύπος PageAreaFilter εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | Αρχικοποιεί ένα νέο PageAreaFilter για τη διαγραφή μιας συγκεκριμένης περιοχής. |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | Το ορθογώνιο (θέση επάνω‑αριστερά και μέγεθος της περιοχής) σε μια σελίδα. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
