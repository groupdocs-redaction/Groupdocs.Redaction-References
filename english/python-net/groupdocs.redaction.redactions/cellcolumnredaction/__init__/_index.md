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
from groupdocs.redaction.redactions import CellFilter

# Define a filter for column 2 in the first worksheet
cell_filter = CellFilter()
cell_filter.column_index = 2
cell_filter.work_sheet_name = "Sheet1"

# Create a redaction that replaces matches of the regex with a placeholder
redaction = CellColumnRedaction(
    cell_filter,
    r"\bsecret\b",
    ReplacementOptions("[REDACTED]")
)

with Redactor("spreadsheet.xlsx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### See Also
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
