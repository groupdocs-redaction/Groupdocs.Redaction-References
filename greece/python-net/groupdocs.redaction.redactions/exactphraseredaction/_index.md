---
title: "Κλάση ExactPhraseRedaction"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια κειμενική απόκρυψη που αντικαθιστά μια ακριβή φράση στο κείμενο του εγγράφου, χωρίς διάκριση πεζών-κεφαλαίων από προεπιλογή."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

Αντιπροσωπεύει μια κειμενική απόκρυψη που αντικαθιστά μια ακριβή φράση στο κείμενο του εγγράφου, χωρίς διάκριση πεζών-κεφαλαίων από προεπιλογή.

Μάθετε περισσότερα:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

Ο τύπος ExactPhraseRedaction εκθέτει τα παρακάτω μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | Αρχικοποιεί ένα νέο αντίγραφο του ExactPhraseRedaction σε λειτουργία χωρίς διάκριση πεζών‑κεφαλαίων. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | Αρχικοποιεί ένα νέο αντίγραφο ExactPhraseRedaction. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | Εφαρμόζει τη redaction σε ένα δεδομένο αντικείμενο μορφής. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | Η περιγραφή της διαγραφής, που περιέχει το όνομα της διαγραφής και τις παραμέτρους. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | Η τιμή που υποδεικνύει εάν η αναζήτηση είναι ευαίσθητη σε πεζά‑κεφαλαία. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | Η σημαία κατεύθυνσης κειμένου που υποδεικνύει εάν το κείμενο είναι από δεξιά προς αριστερά. Η προεπιλογή είναι False. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | Η συμβολοσειρά για αναζήτηση και αντικατάσταση. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Το αντικείμενο [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) που καθορίζει τον τύπο κειμενικής αντικατάστασης. (κληρονομείται από το [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Η υλοποίηση IOcrConnector που χρησιμοποιείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο. (κληρονομείται από το [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # αντικατάσταση με διάκριση πεζών‑κεφαλαίων
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν `ExactPhraseRedaction`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
