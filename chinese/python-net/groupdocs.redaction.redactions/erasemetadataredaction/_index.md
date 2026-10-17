---
title: "EraseMetadataRedaction 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示一种元数据编辑，它从文档中擦除所有元数据或匹配特定 MetadataFilters 的元数据。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

表示一种元数据编辑，它从文档中擦除所有元数据或匹配特定 MetadataFilters 的元数据。

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

该 EraseMetadataRedaction 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | 初始化 EraseMetadataRedaction 类的新实例，擦除所有元数据。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | 初始化 EraseMetadataRedaction 的新实例，擦除匹配指定 `MetadataFilters` 的元数据。 |

### 方法
| 方法 | 描述 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | 将编辑应用于给定的格式实例。（继承自 [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)） |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | （继承自 [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)） |

### 属性
| 属性 | 描述 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | 编辑的描述及其参数。 |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | 用于选择全部或特定元数据（如 Author 或 Company）的过滤器。（继承自 [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)） |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # 擦除所有元数据
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # 仅擦除作者字段
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
使用 `EraseMetadataRedaction` 的任务指南：

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 另请参阅
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
