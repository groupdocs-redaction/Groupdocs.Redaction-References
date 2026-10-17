---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化一个新的 PageAreaRedaction 实例。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

初始化一个新的 PageAreaRedaction 实例。

```python
def __init__(self, regex, options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 用于搜索和替换的正则表达式。 |
| options | `ReplacementOptions` | 替换选项（文本、颜色）。 |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(r"\d{3}-\d{2}-\d{4}", ReplacementOptions("[SSN]"))
    )
    redactor.save()
```

## __init__ {#regex-options-image_options}

初始化一个新的 PageAreaRedaction。

```python
def __init__(self, regex, options, image_options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 用于搜索和替换的正则表达式。 |
| options | `ReplacementOptions` | 替换选项（文本、颜色）。 |
| image_options | `RegionReplacementOptions` | 替换选项（图像区域）。 |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

redactor = Redactor("scan.pdf")
redactor.apply(
    PageAreaRedaction(
        r"\d{3}-\d{2}-\d{4}",
        ReplacementOptions("[SSN]"),
        RegionReplacementOptions(Color.BLACK, Size(120, 20))
    )
)
redactor.save()
```

### 另请参阅
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
