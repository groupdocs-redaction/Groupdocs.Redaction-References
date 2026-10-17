---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny RemovePageRedaction."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

Initierar en ny RemovePageRedaction.

```python
def __init__(self, origin, index, count):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Sök referensposition, början eller slutet av ett dokument. |
| index | `int` | Startpositionsindex (0‑baserad). |
| count | `int` | Antal sidor att ta bort. |

### Exempel

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Ta bort 3 sidor med början från den andra sidan (noll‑baserat index 1)
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### Se även
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
