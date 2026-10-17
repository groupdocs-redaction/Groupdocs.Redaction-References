---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ينشئ مثيلاً جديداً من CellColumnRedaction."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

ينشئ مثيلاً جديداً من CellColumnRedaction.

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| filter | `CellFilter` | مرشح العمود وورقة العمل. |
| reg_ex | `System.Text.RegularExpressions.Regex` | تعبير نمطي للبحث والاستبدال. |
| options | `ReplacementOptions` | خيارات الاستبدال. |

### مثال

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

### انظر أيضًا
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
