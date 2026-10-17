---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化 DeleteAnnotationRedaction 类的新实例，使用删除所有注释（匹配全部）的设置。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

初始化 DeleteAnnotationRedaction 类的新实例，使用删除所有注释（匹配全部）的设置。

```python
def __init__(self):
    ...
```

### 示例

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# 删除所有注释
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

初始化 DeleteAnnotationRedaction 类的新实例，删除匹配给定表达式的注释。

```python
def __init__(self, pattern):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| pattern | `str` | 正则表达式。 |

### 示例

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# 删除包含单词 "internal" 的注释（不区分大小写）
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

初始化 DeleteAnnotationRedaction 类的新实例，删除匹配给定表达式的注释。

```python
def __init__(self, regex):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 正则表达式。 |

### 示例

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# 删除内容匹配正则表达式的注释（不区分大小写）
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### 另请参阅
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
