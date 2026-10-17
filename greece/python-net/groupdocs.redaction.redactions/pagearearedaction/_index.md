---
title: "Κλάση PageAreaRedaction"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια σύνθετη κειμενική επεξεργασία που επηρεάζει κείμενο, εικόνες και σημειώσεις σε μια περιοχή της σελίδας."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

Αντιπροσωπεύει μια σύνθετη κειμενική επεξεργασία που επηρεάζει κείμενο, εικόνες και σημειώσεις σε μια περιοχή της σελίδας.

Μάθετε περισσότερα

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

Ο τύπος PageAreaRedaction εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | Αρχικοποιεί ένα νέο αντικείμενο PageAreaRedaction. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | Αρχικοποιεί ένα νέο PageAreaRedaction. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | Εφαρμόζει τη redaction σε ένα δεδομένο αντικείμενο μορφής. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | Οι επιλογές RegionReplacementOptions με παραμέτρους χρώματος και περιοχής. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Το αντικείμενο [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) που καθορίζει τον τύπο κειμενικής αντικατάστασης. (κληρονομείται από το [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | Η περιγραφή της διαγραφής, που περιέχει το όνομά της και τις παραμέτρους. (κληρονομείται από [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Η υλοποίηση IOcrConnector που χρησιμοποιείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο. (κληρονομείται από το [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Το πρότυπο κανονικής έκφρασης που χρησιμοποιείται για την αντιστοίχιση. (κληρονομείται από [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(
            r"\d{3}-\d{2}-\d{4}",
            ReplacementOptions("[SSN]"),
            RegionReplacementOptions(Color.BLACK, Size(120, 20))
        )
    )
    redactor.save()
```

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
