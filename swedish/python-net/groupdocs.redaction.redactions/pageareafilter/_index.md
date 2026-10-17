---
title: "PageAreaFilter-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar ett raderingsfilter som anger ett område inom en sida i ett dokument för att tillämpa radering."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

Representerar ett raderingsfilter som anger ett område inom en sida i ett dokument för att tillämpa radering.

Läs mer

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

PageAreaFilter-typen exponerar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | Initierar en ny PageAreaFilter för att radera ett specifikt område. |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | Rektangeln (övre vänstra positionen och storleken på området) på en sida. |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### Se även
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
