---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "在不区分大小写模式下初始化 ExactPhraseRedaction 的新实例。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

在不区分大小写模式下初始化 ExactPhraseRedaction 的新实例。

```python
def __init__(self, search_phrase, options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| search_phrase | `str` | 用于搜索和替换的字符串。 |
| options | `ReplacementOptions` | 替换选项（文本、颜色）。 |

### 示例

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# 将 "John Doe" 的出现替换为 "[CUSTOMER]"（不区分大小写）
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

初始化一个新的 ExactPhraseRedaction 实例。

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| search_phrase | `str` | 用于搜索和替换的字符串。 |
| is_case_sensitive | `bool` | 如果需要区分大小写搜索，则为 True。 |
| options | `ReplacementOptions` | 替换选项（文本、颜色）。 |

### 示例

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# 不区分大小写的精确短语脱敏
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# 区分大小写的精确短语脱敏
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### 另请参阅
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
