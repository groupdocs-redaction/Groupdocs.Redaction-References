---
title: "Κλάση ImageAreaRedaction"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια επεξεργασία που τοποθετεί ένα χρωματιστό ορθογώνιο σε μια δοσμένη περιοχή ενός εγγράφου εικόνας."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

Αντιπροσωπεύει μια επεξεργασία που τοποθετεί ένα χρωματιστό ορθογώνιο σε μια δοσμένη περιοχή ενός εγγράφου εικόνας.

Μάθετε περισσότερα:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Ο τύπος ImageAreaRedaction εκθέτει τα παρακάτω μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | Αρχικοποιεί ένα νέο ImageAreaRedaction για τη διαγραφή μιας συγκεκριμένης ορθογώνιας περιοχής. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | Εφαρμόζει τη redaction σε ένα δεδομένο αντικείμενο μορφής. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to_document_format_instance/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | Η περιγραφή της redaction, που περιλαμβάνει το όνομα και τις παραμέτρους της. |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | Οι επιλογές RegionReplacementOptions με παραμέτρους χρώματος και περιοχής. |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | Η θέση πάνω‑αριστερά της περιοχής που θα αφαιρεθεί. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

point = Point(516, 311)
size = Size(170, 35)
color = Color.from_argb(255, 0, 0, 255)  # blue
options = RegionReplacementOptions(color, size)
redaction = ImageAreaRedaction(point, options)

with Redactor("D:\\test.jpg") as redactor:
    result = redactor.apply(redaction)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν `ImageAreaRedaction`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
