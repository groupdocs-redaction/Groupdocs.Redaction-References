---
title: "Κλάση PageRangeFilter"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει φίλτρο επεξεργασίας, ορίζοντας εύρος σελίδων μέσα σε ένα έγγραφο για την εφαρμογή της επεξεργασίας."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

Αντιπροσωπεύει φίλτρο επεξεργασίας, ορίζοντας εύρος σελίδων μέσα σε ένα έγγραφο για την εφαρμογή της επεξεργασίας.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

Ο τύπος PageRangeFilter εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | Αρχικοποιεί ένα νέο RemovePageRedaction. |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | Ο αριθμός των σελίδων προς αφαίρεση. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | Ο δείκτης θέσης εκκίνησης (βάση 0). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | Η θέση αναφοράς αναζήτησης, είτε η αρχή είτε το τέλος ενός εγγράφου. |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# Ορίστε ένα φίλτρο που στοχεύει στην τελευταία σελίδα και στην προηγούμενη.
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# Το φίλτρο μπορεί να συνδυαστεί με άλλα φίλτρα, π.χ., PageAreaFilter,
# και να περάσει στο ReplacementOptions.Filters κατά τη διαμόρφωση μιας διαγραφής.
```

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
