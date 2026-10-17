---
title: "ReplacementOptions 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示匹配文本替换的选项。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

表示匹配文本替换的选项。

了解更多

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

ReplacementOptions 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | 使用指定的替换文本初始化 ReplacementOptions 的新实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | 使用彩色矩形作为选项初始化 ReplacementOptions 类的新实例。 |

### 属性
| 属性 | 描述 |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | 替换操作：绘制框或替换文本。 |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | `ReplacementType.draw_box` 选项的颜色（否则将被忽略）。 |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | 自定义遮蔽处理程序，允许用户定义自己的遮蔽逻辑。 |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | 此遮蔽要应用的过滤器数组。 |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | 文本替换值。 |

### 示例

```python
from groupdocs.redaction.redactions import ReplacementOptions

# 将匹配的文本替换为占位符 "[X]"
repl_opt = ReplacementOptions("[X]")
```

### Guides
使用 `ReplacementOptions` 的任务指南：

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 另请参阅
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
