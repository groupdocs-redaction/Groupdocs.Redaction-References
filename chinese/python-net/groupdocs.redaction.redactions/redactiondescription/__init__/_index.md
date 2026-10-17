---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化 RedactionDescription 类的新实例，不包含替换信息。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

初始化 RedactionDescription 类的新实例，不包含替换信息。

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| redaction_type | `RedactionType` | 被编辑的数据类型。 |
| action_type | `RedactionActionType` | 对这些数据执行的操作。 |
| original_text | `str` | 匹配的文本、注释或批注正文。 |

## __init__ {#redaction_type-action_type-original_text-replacement}

初始化 RedactionDescription 类的新实例，包含替换信息。

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| redaction_type | `RedactionType` | 被编辑的数据类型。 |
| action_type | `RedactionActionType` | 对这些数据执行的操作。 |
| original_text | `str` | 匹配的文本、注释或批注正文。 |
| replacement | `TextReplacement` | 替换文本、匹配的文本及其在原始字符串中的位置。 |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

初始化带有图像区域替换信息的 RedactionDescription。

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| redaction_type | `RedactionType` | 被编辑的数据类型。 |
| action_type | `RedactionActionType` | 对这些数据执行的操作。 |
| image_area_replacement | `RegionReplacementOptions` | 图像区域替换信息。 |
| image_details | `str` | 图像文本描述，默认是空字符串。 |

### 另请参阅
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
