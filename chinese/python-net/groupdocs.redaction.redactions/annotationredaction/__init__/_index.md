---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "使用正则表达式模式和替换文本初始化新的 AnnotationRedaction。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

使用正则表达式模式和替换文本初始化新的 AnnotationRedaction。

```python
def __init__(self, pattern, replacement):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| pattern | `str` | 用于匹配的正则表达式。 |
| replacement | `str` | 匹配文本的文本替换。 |

### 示例

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# 在注释文本中编辑单词 "approved"
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

初始化 [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) 的新实例。

```python
def __init__(self, regex, replacement):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 用于匹配的正则表达式。 |
| replacement | `str` | 匹配文本的文本替换。 |

### 示例

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# 编辑单词 "approved"（不区分大小写）并将其替换为 "[REVIEW]"
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### 另请参阅
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
