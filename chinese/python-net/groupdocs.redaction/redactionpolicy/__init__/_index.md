---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化一个新的 RedactionPolicy 实例。"
type: docs
url: /zh/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

初始化一个新的 RedactionPolicy 实例。

```python
def __init__(self):
    ...
```

### 示例

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

使用特定的编辑列表初始化一个新的 RedactionPolicy。

```python
def __init__(self, redactions):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| redactions | `list[Redaction]` | 策略的 redactions 数组。 |

### 示例

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### 另请参阅
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
