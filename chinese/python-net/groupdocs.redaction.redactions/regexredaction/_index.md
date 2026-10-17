---
title: "RegexRedaction 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示一种文本编辑，通过匹配提供的正则表达式搜索并替换文档中的文本。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

表示一种文本编辑，通过匹配提供的正则表达式搜索并替换文档中的文本。

了解更多

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

RegexRedaction 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | 初始化 RegexRedaction 的新实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | 初始化新的 RegexRedaction 实例。 |

### 方法
| 方法 | 描述 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | 将 redaction 应用于给定的格式实例。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### 属性
| 属性 | 描述 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | redaction 的描述，包含其名称和参数。 |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | 用于匹配的正则表达式模式。 |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | 指定文本替换类型的 [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) 实例。（继承自 [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)） |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | 用于从图形内容中提取文本的 IOcrConnector 实现。（继承自 [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)） |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # 替换为文本
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # 替换为蓝色实心矩形
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
使用 `RegexRedaction` 的任务指南：

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 另请参阅
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
