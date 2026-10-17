---
title: "Κλάση RegexRedaction"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια κειμενική επεξεργασία που αναζητά και αντικαθιστά κείμενο στο έγγραφο ταιριάζοντας με την παρεχόμενη κανονική έκφραση."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

Αντιπροσωπεύει μια κειμενική επεξεργασία που αναζητά και αντικαθιστά κείμενο στο έγγραφο ταιριάζοντας με την παρεχόμενη κανονική έκφραση.

Μάθετε περισσότερα

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

Ο τύπος RegexRedaction εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | Αρχικοποιεί ένα νέο αντικείμενο του RegexRedaction. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | Αρχικοποιεί ένα νέο αντικείμενο RegexRedaction. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | Εφαρμόζει τη redaction σε ένα δεδομένο αντικείμενο μορφής. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | Η περιγραφή της redaction, που περιλαμβάνει το όνομα και τις παραμέτρους της. |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Το πρότυπο κανονικής έκφρασης που χρησιμοποιείται για την αντιστοίχιση. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Το αντικείμενο [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) που καθορίζει τον τύπο κειμενικής αντικατάστασης. (κληρονομείται από το [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Η υλοποίηση IOcrConnector που χρησιμοποιείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο. (κληρονομείται από το [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # αντικατάσταση με κείμενο
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # αντικατάσταση με μπλε στερεό ορθογώνιο
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν το `RegexRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
