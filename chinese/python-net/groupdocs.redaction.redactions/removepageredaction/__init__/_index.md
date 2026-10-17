---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化一个新的 RemovePageRedaction。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

初始化一个新的 RemovePageRedaction。

```python
def __init__(self, origin, index, count):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| origin | `PageSeekOrigin` | 查找参考位置，文档的开头或结尾。 |
| index | `int` | 起始位置索引（从 0 开始）。 |
| count | `int` | 要删除的页数。 |

### 示例

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# 从第二页（零基索引 1）起删除 3 页
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### 另请参阅
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
