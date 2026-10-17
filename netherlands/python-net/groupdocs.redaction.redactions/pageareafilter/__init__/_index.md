---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuwe PageAreaFilter voor het redigeren van een specifiek gebied."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

Initialiseert een nieuwe PageAreaFilter voor het redigeren van een specifiek gebied.

```python
def __init__(self, top_left, size):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Coördinaten van het gebied linksboven. |
| size | `System.Drawing.Size` | Grootte en kleur van het gebied. |

### Voorbeeld

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### Zie ook
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
