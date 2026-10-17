---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化一个新的 RegionReplacementOptions 实例。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

初始化一个新的 RegionReplacementOptions 实例。

```python
def __init__(self, fill_color, size):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | 用于填充区域的颜色。 |
| size | `System.Drawing.Size` | 已填充区域的大小。 |

### 示例

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

初始化一个新的 RegionReplacementOptions 类实例，其大小匹配给定的文本。

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | 用于填充区域的颜色。 |
| font | `System.Drawing.Font` | 期望的文本字体。 |
| expected_text | `str` | 期望的文本。 |

### 另请参阅
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
