---
title: "RegionReplacementOptions κλάση"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει παραμέτρους χρώματος και περιοχής για αντικατάσταση περιοχής εικόνας."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

Αντιπροσωπεύει παραμέτρους χρώματος και περιοχής για αντικατάσταση περιοχής εικόνας.

Μάθετε περισσότερα:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Ο τύπος RegionReplacementOptions εκθέτει τα παρακάτω μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | Αρχικοποιεί ένα νέο αντικείμενο RegionReplacementOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RegionReplacementOptions του οποίου το μέγεθος ταιριάζει με το δεδομένο κείμενο. |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | Το χρώμα που χρησιμοποιείται για τη γέμιση της διαγραμμένης περιοχής. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | Το πλάτος και το ύψος του ορθογωνίου. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # Ορίστε τη θέση πάνω‑αριστερά της περιοχής που θα αντικατασταθεί
    point = Point(516, 311)
    # Ορίστε το μέγεθος της περιοχής που θα αντικατασταθεί
    size = Size(170, 35)
    # Χρησιμοποιήστε ένα συμπαγές μαύρο ορθογώνιο ως αντικατάσταση
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν `RegionReplacementOptions`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
