---
title: "RegionReplacementOptions 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示图像区域替换的颜色和区域参数。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

表示图像区域替换的颜色和区域参数。

了解更多：
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

该 RegionReplacementOptions 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | 初始化一个新的 RegionReplacementOptions 实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | 初始化一个新的 RegionReplacementOptions 类实例，其大小匹配给定的文本。 |

### 属性
| 属性 | 描述 |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | 用于填充已编辑区域的颜色。 |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | 矩形的宽度和高度。 |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # 定义要替换区域的左上位置
    point = Point(516, 311)
    # 定义要替换区域的大小
    size = Size(170, 35)
    # 使用实心黑色矩形作为替换
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
使用 `RegionReplacementOptions` 的任务指南：

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### 另请参阅
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
