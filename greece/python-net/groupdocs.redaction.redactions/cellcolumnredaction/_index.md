---
title: "κλάση CellColumnRedaction"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια κειμενική απόκρυψη που αντικαθιστά το κείμενο σε ένα έγγραφο λογιστικού φύλλου (CSV, Excel κ.λπ.)."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/cellcolumnredaction/
is_root: false
weight: 20
---


## CellColumnRedaction class

Αντιπροσωπεύει μια κειμενική απόκρυψη που αντικαθιστά το κείμενο σε ένα έγγραφο λογιστικού φύλλου (CSV, Excel κ.λπ.).

- Learn more: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about spreadsheet redactions: https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/

Ο τύπος CellColumnRedaction εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/#filter-reg_ex-options) | Αρχικοποιεί ένα νέο CellColumnRedaction. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to/#format_instance) | Εφαρμόζει τη redaction σε ένα δεδομένο αντικείμενο μορφής. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to_document_format_instance/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/description/) | Η περιγραφή της redaction, που περιλαμβάνει το όνομα και τις παραμέτρους της. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/filter/) | Το φίλτρο στήλης και φύλλου εργασίας. |
| [pattern](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/pattern/) | Το πρότυπο κανονικής έκφρασης για την αντιστοίχιση. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Το αντικείμενο [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) που καθορίζει τον τύπο κειμενικής αντικατάστασης. (κληρονομείται από το [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Η υλοποίηση IOcrConnector που χρησιμοποιείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο. (κληρονομείται από το [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.redaction.filters import CellFilter

with Redactor("Sales in September.xlsx") as redactor:
    filter = CellFilter(column_index=1, worksheet_name="Customers")
    regex = r"^\w+([-+.']\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$"
    redactor.apply(CellColumnRedaction(filter, regex, ReplacementOptions("[customer email]")))
    redactor.save()
```

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
