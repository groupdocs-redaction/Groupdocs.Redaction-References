---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new CellColumnRedaction."
type: docs
url: /python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

Initializes a new CellColumnRedaction.

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| filter | `CellFilter` | Column and worksheet filter. |
| reg_ex | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace. |
| options | `ReplacementOptions` | Replacement options. |

### Example

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

### See Also
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
