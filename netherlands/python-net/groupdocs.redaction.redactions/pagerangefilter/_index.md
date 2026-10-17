---
title: "PageRangeFilter klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een redactiefilter voor, waarbij een paginabereik binnen een document wordt ingesteld om redacties toe te passen."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

Stelt een redactiefilter voor, waarbij een paginabereik binnen een document wordt ingesteld om redacties toe te passen.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

Het type PageRangeFilter exposeert de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | Initialiseert een nieuwe RemovePageRedaction. |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | Het aantal te verwijderen pagina's. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | De startpositie‑index (0-gebaseerd). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | De referentiepositie voor zoeken, ofwel het begin of het einde van een document. |

### Voorbeeld

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# Definieer een filter dat zich richt op de laatste pagina en de daarvoor gelegen pagina
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# Het filter kan worden gecombineerd met andere filters, bijv., PageAreaFilter,
# en doorgegeven aan ReplacementOptions.Filters bij het configureren van een redactie.
```

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
