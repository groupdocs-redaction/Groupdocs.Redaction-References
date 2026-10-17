---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny PageAreaFilter för att radera ett specifikt område."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

Initierar en ny PageAreaFilter för att radera ett specifikt område.

```python
def __init__(self, top_left, size):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Koordinater för område uppe till vänster. |
| size | `System.Drawing.Size` | Områdets storlek och färg. |

### Exempel

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### Se även
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
