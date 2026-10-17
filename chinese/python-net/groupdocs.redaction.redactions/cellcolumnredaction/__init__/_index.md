---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化新的 CellColumnRedaction。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

初始化新的 CellColumnRedaction。

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| filter | `CellFilter` | 列和工作表过滤器。 |
| reg_ex | `System.Text.RegularExpressions.Regex` | 用于搜索和替换的正则表达式。 |
| options | `ReplacementOptions` | 替换选项。 |

### 示例

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

### 另请参阅
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
