---
title: "PageRangeFilter Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt einen Redaktionsfilter dar, der einen Seitenbereich innerhalb eines Dokuments festlegt, in dem die Redaktion angewendet wird."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

Stellt einen Redaktionsfilter dar, der einen Seitenbereich innerhalb eines Dokuments festlegt, in dem die Redaktion angewendet wird.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

Der Typ PageRangeFilter stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | Initialisiert eine neue RemovePageRedaction. |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | Die Anzahl der zu entfernenden Seiten. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | Der Startpositionsindex (0-basiert). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | Die Referenzposition für das Suchen, entweder der Anfang oder das Ende eines Dokuments. |

### Beispiel

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# Definieren Sie einen Filter, der die letzte Seite und die davor liegende Seite anvisiert
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# Der Filter kann mit anderen Filtern kombiniert werden, z. B. PageAreaFilter,
# und an ReplacementOptions.Filters übergeben werden, wenn eine Redaktion konfiguriert wird.
```

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
