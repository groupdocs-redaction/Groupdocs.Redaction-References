---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化 EraseMetadataRedaction 类的新实例，擦除所有元数据。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

初始化 EraseMetadataRedaction 类的新实例，擦除所有元数据。

```python
def __init__(self):
    ...
```

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

初始化 EraseMetadataRedaction 的新实例，擦除匹配指定 `MetadataFilters` 的元数据。

```python
def __init__(self, filter):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| filter | `MetadataFilters` | 用于擦除的元数据过滤器。 |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # 擦除所有元数据
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # 仅擦除作者元数据字段
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### 另请参阅
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
