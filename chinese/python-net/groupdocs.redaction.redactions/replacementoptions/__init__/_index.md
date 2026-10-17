---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "使用指定的替换文本初始化 ReplacementOptions 的新实例。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

使用指定的替换文本初始化 ReplacementOptions 的新实例。

```python
def __init__(self, replacement):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| replacement | `str` | 文本替换。 |

### 示例

```python
from groupdocs.redaction.redactions import ReplacementOptions

# 将匹配的文本替换为 "[REDACTED]"
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

使用彩色矩形作为选项初始化 ReplacementOptions 类的新实例。

```python
def __init__(self, color):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| color | `System.Drawing.Color` | 矩形颜色。 |

### 另请参阅
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
