---
title: "PageAreaFilter klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een redactiefilter voor, waarbij een gebied binnen een pagina van een document wordt ingesteld om redacties toe te passen."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

Stelt een redactiefilter voor, waarbij een gebied binnen een pagina van een document wordt ingesteld om redacties toe te passen.

Meer informatie

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Het type PageAreaFilter exposeert de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | Initialiseert een nieuwe PageAreaFilter voor het redigeren van een specifiek gebied. |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | De rechthoek (positie linksboven en grootte van het gebied) op een pagina. |

### Voorbeeld

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

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
