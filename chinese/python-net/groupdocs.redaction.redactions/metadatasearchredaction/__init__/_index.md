---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "使用值匹配已编辑的项，初始化 MetadataSearchRedaction 类的新实例。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

使用值匹配已编辑的项，初始化 MetadataSearchRedaction 类的新实例。

```python
def __init__(self, value_pattern, replacement):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| value_pattern | `str` | 用于搜索和替换的正则表达式 |
| replacement | `str` | 文本替换 |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

使用项目名称和值匹配已编辑的项，初始化 MetadataSearchRedaction 的新实例。

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| value_pattern | `str` | 用于搜索和替换元数据项值的正则表达式。 |
| replacement | `str` | 文本替换。 |
| key_pattern | `str` | 用于搜索和替换元数据项名称的正则表达式。 |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # 替换元数据值中出现的任何电子邮件地址
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

使用值匹配已编辑的项，初始化 MetadataSearchRedaction 类的新实例。

```python
def __init__(self, value_regex, replacement):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | 用于搜索和替换的正则表达式。 |
| replacement | `str` | 文本替换。 |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# 对元数据中的任何电子邮件地址进行脱敏
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

使用项目名称和值匹配已编辑的项，初始化 MetadataSearchRedaction 的新实例。

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | 用于搜索和替换元数据项值的正则表达式。 |
| replacement | `str` | 文本替换。 |
| key_regex | `System.Text.RegularExpressions.Regex` | 用于搜索和替换元数据项名称的正则表达式。 |

### 示例

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# 对元数据值中的电子邮件地址进行脱敏
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### 另请参阅
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
