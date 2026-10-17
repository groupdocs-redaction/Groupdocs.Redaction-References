---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化一个用于遮蔽特定区域的新 PageAreaFilter。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

初始化一个用于遮蔽特定区域的新 PageAreaFilter。

```python
def __init__(self, top_left, size):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | 左上角区域坐标。 |
| size | `System.Drawing.Size` | 区域大小和颜色。 |

### 示例

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### 另请参阅
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
