---
title: "PageRangeFilter-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar ett raderingsfilter som anger sidintervall i ett dokument för att tillämpa radering."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

Representerar ett raderingsfilter som anger sidintervall i ett dokument för att tillämpa radering.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

PageRangeFilter-typen exponerar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | Initierar en ny RemovePageRedaction. |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | Antalet sidor att ta bort. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | Startpositionsindexet (0-baserat). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | Sökreferenspositionen, antingen början eller slutet av ett dokument. |

### Exempel

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# Definiera ett filter som riktar sig mot den sista sidan och föregående sida
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# Filtret kan kombineras med andra filter, t.ex. PageAreaFilter,
# och skickas till ReplacementOptions.Filters när en radering konfigureras.
```

### Se även
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
