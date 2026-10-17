---
title: "MetadataSearchRedaction 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示一种使用正则表达式搜索并编辑元数据的元数据编辑，可匹配键和/或值。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

表示一种使用正则表达式搜索并编辑元数据的元数据编辑，可匹配键和/或值。

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

MetadataSearchRedaction 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | 使用值匹配已编辑的项，初始化 MetadataSearchRedaction 类的新实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | 使用项目名称和值匹配已编辑的项，初始化 MetadataSearchRedaction 的新实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | 使用值匹配已编辑的项，初始化 MetadataSearchRedaction 类的新实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | 使用项目名称和值匹配已编辑的项，初始化 MetadataSearchRedaction 的新实例。 |

### 方法
| 方法 | 描述 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | 将编辑应用于给定的格式实例。（继承自 [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)） |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | （继承自 [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)） |

### 属性
| 属性 | 描述 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | redaction 的描述，包含其名称和参数。 |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | 用于匹配元数据项名称（键）的正则表达式。 |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | 文本替换值。 |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | 用于匹配元数据项值文本的正则表达式。 |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | 用于选择全部或特定元数据（如 Author 或 Company）的过滤器。（继承自 [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)） |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # 编辑匹配该模式的任何元数据值
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
使用 `MetadataSearchRedaction` 的任务指南：

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### 另请参阅
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
