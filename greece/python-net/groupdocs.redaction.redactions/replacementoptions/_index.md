---
title: "Κλάση ReplacementOptions"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει επιλογές για την αντικατάσταση ταιριαστού κειμένου."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

Αντιπροσωπεύει επιλογές για την αντικατάσταση ταιριαστού κειμένου.

Μάθετε περισσότερα

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Ο τύπος ReplacementOptions εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | Αρχικοποιεί ένα νέο αντικείμενο του ReplacementOptions με το καθορισμένο κείμενο αντικατάστασης. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ReplacementOptions με χρωματιστό ορθογώνιο ως επιλογή. |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | Η ενέργεια αντικατάστασης: σχεδίαση πλαισίου ή αντικατάσταση κειμένου. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | Το χρώμα για την επιλογή `ReplacementType.draw_box` (αγνοείται διαφορετικά). |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | Ο προσαρμοσμένος διαχειριστής διαγραφής που επιτρέπει στους χρήστες να ορίσουν τη δική τους λογική διαγραφής. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | Ο πίνακας των φίλτρων που θα εφαρμοστούν με αυτή τη διαγραφή. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | Η τιμή κειμενικής αντικατάστασης. |

### Παράδειγμα

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Αντικαταστήστε το ταιριασμένο κείμενο με το σύμβολο κράτησης θέσης "[X]"
repl_opt = ReplacementOptions("[X]")
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν το `ReplacementOptions`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
