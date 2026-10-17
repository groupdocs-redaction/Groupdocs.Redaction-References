---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny CellColumnRedaction."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

Initierar en ny CellColumnRedaction.

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| filter | `CellFilter` | Kolumn- och kalkylbladsfilter. |
| reg_ex | `System.Text.RegularExpressions.Regex` | Reguljärt uttryck för att söka och ersätta. |
| options | `ReplacementOptions` | Ersättningsalternativ. |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("spreadsheet.xlsx") as redactor:
    redactor.apply(
        CellColumnRedaction(
            CellFilter(worksheet="Sheet1", column=2),
            r"\bsecret\b",
            ReplacementOptions(Color.BLACK)
        )
    )
    redactor.save()
```

### Se även
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
