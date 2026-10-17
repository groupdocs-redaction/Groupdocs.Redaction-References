---
title: "Klasse PageAreaFilter"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt einen Redaktionsfilter dar, der einen Bereich innerhalb einer Seite eines Dokuments festlegt, in dem die Redaktion angewendet wird."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

Stellt einen Redaktionsfilter dar, der einen Bereich innerhalb einer Seite eines Dokuments festlegt, in dem die Redaktion angewendet wird.

Mehr erfahren

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Der Typ PageAreaFilter stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | Initialisiert einen neuen PageAreaFilter zum Schwärzen eines bestimmten Bereichs. |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | Das Rechteck (obere linke Position und Größe des Bereichs) auf einer Seite. |

### Beispiel

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

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
