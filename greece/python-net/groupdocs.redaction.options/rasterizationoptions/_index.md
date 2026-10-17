---
title: "Κλάση RasterizationOptions"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Παρέχει επιλογές για τη μετατροπή αρχείων σε PDF."
type: docs
url: /el/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

Παρέχει επιλογές για τη μετατροπή αρχείων σε PDF.

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

Ο τύπος RasterizationOptions εκθέτει τα παρακάτω μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | Αρχικοποιεί μια νέα παρουσία. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | Καταχωρεί μια προχωρημένη επιλογή rasterization για εφαρμογή. |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | Καταχωρεί μια προχωρημένη επιλογή rasterization για εφαρμογή. |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | Το επίπεδο συμμόρφωσης PDF. |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | Η σημαία ενεργοποίησης υποδεικνύει εάν όλες οι σελίδες του εγγράφου μετατρέπονται σε εικόνες και τοποθετούνται σε ένα ενιαίο αρχείο PDF. Η προεπιλογή είναι True· ορίστε σε False για να αποφύγετε τη ραστεροποίηση. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | Ο δείκτης είναι True εάν έχουν οριστεί προχωρημένες επιλογές ραστεροποίησης. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | Ο αριθμός των σελίδων που θα μετατραπούν σε PDF. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | Το ευρετήριο της πρώτης σελίδας (από το 0) που θα μετατραπεί σε PDF. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import RasterizationOptions, PdfComplianceLevel

with Redactor("SomePresentation.pptx") as redactor:
    ro = RasterizationOptions()
    ro.page_index = 0          # first slide
    ro.page_count = 1
    ro.compliance = PdfComplianceLevel.PdfA1a
    redactor.save("PresentationFirstSlide.pdf", ro)
```

### Δείτε επίσης
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
