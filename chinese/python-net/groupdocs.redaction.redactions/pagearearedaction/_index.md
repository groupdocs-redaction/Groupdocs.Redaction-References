---
title: "PageAreaRedaction 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示一种复杂的文本编辑，影响页面区域内的文字、图像和批注。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

表示一种复杂的文本编辑，影响页面区域内的文字、图像和批注。

了解更多

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

PageAreaRedaction 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | 初始化一个新的 PageAreaRedaction 实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | 初始化一个新的 PageAreaRedaction。 |

### 方法
| 方法 | 描述 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | 将 redaction 应用于给定的格式实例。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### 属性
| 属性 | 描述 |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | RegionReplacementOptions 选项，带有颜色和区域参数。 |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | 指定文本替换类型的 [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) 实例。（继承自 [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)） |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | redaction 的描述，包含其名称和参数。（继承自 [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)） |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | 用于从图形内容中提取文本的 IOcrConnector 实现。（继承自 [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)） |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | 用于匹配的正则表达式模式。（继承自 [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)） |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(
            r"\d{3}-\d{2}-\d{4}",
            ReplacementOptions("[SSN]"),
            RegionReplacementOptions(Color.BLACK, Size(120, 20))
        )
    )
    redactor.save()
```

### 另请参阅
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
