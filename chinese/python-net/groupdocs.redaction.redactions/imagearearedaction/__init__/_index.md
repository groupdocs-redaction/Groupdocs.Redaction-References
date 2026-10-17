---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化用于编辑特定矩形区域的新 ImageAreaRedaction。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

初始化用于编辑特定矩形区域的新 ImageAreaRedaction。

```python
def __init__(self, top_left, options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | 左上角区域坐标。 |
| options | `RegionReplacementOptions` | 区域大小和颜色。 |

### 示例

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# 定义要编辑区域的左上角
top_left = Point(385, 485)
# 定义编辑区域的大小和颜色
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# 创建编辑对象
redaction = ImageAreaRedaction(top_left, region_options)
```

### 另请参阅
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
