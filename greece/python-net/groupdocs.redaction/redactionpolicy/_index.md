---
title: "Κλάση RedactionPolicy"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια πολιτική εξαγνισμού, που περιέχει ένα σύνολο συγκεκριμένων επεμβάσεων προς εφαρμογή."
type: docs
url: /el/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

Αντιπροσωπεύει μια πολιτική εξαγνισμού, που περιέχει ένα σύνολο συγκεκριμένων επεμβάσεων προς εφαρμογή.

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

Ο τύπος RedactionPolicy εκθέτει τα παρακάτω μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | Αρχικοποιεί ένα νέο αντικείμενο RedactionPolicy. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | Αρχικοποιεί ένα νέο RedactionPolicy με μια συγκεκριμένη λίστα διαγραφών. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | Φορτώνει ένα RedactionPolicy από αρχείο XML. |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | Φορτώνει ένα αντικείμενο RedactionPolicy από ροή που περιέχει διαμόρφωση XML. |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | Αποθηκεύει την πολιτική διαγραφής σε αρχείο. |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | Αποθηκεύει την πολιτική διαγραφής σε ροή. |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | Η λίστα των πλήρως διαμορφωμένων κλάσεων που προέρχονται από [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/). |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# Δημιουργήστε μια επαναχρησιμοποιήσιμη πολιτική στη μνήμη
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# Εφαρμόστε την πολιτική σε ένα έγγραφο
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν `RedactionPolicy`:

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Δείτε επίσης
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
