---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化 RegexRedaction 的新实例。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

初始化 RegexRedaction 的新实例。

```python
def __init__(self, pattern, options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| pattern | `str` | 用于搜索和替换的正则表达式。 |
| options | `ReplacementOptions` | 替换选项（文本、颜色）。 |

### 示例

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

初始化新的 RegexRedaction 实例。

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
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### 另请参阅
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
