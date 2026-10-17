---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert einen neuen PageAreaFilter zum Schwärzen eines bestimmten Bereichs."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

Initialisiert einen neuen PageAreaFilter zum Schwärzen eines bestimmten Bereichs.

```python
def __init__(self, top_left, size):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Koordinaten des oberen linken Bereichs. |
| size | `System.Drawing.Size` | Bereichsgröße und Farbe. |

### Beispiel

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### Siehe auch
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
