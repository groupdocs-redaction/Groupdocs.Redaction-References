---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuwe CellColumnRedaction."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

Initialiseert een nieuwe CellColumnRedaction.

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| filter | `CellFilter` | Kolom- en werkbladfilter. |
| reg_ex | `System.Text.RegularExpressions.Regex` | Reguliere expressie om te zoeken en te vervangen. |
| options | `ReplacementOptions` | Vervangingsopties. |

### Voorbeeld

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

### Zie ook
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
