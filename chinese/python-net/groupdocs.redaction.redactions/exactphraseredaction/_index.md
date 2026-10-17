---
title: "ExactPhraseRedaction 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示一种文本编辑，默认情况下不区分大小写地替换文档文本中的确切短语。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

表示一种文本编辑，默认情况下不区分大小写地替换文档文本中的确切短语。

了解更多：
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

ExactPhraseRedaction 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | 在不区分大小写模式下初始化 ExactPhraseRedaction 的新实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | 初始化一个新的 ExactPhraseRedaction 实例。 |

### 方法
| 方法 | 描述 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | 将 redaction 应用于给定的格式实例。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### 属性
| 属性 | 描述 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | 编辑的描述，包含编辑名称和参数。 |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | 指示搜索是否区分大小写的值。 |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | 指示文本方向是否从右到左的标志。默认值为 False。 |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | 用于搜索和替换的字符串。 |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | 指定文本替换类型的 [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) 实例。（继承自 [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)） |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | 用于从图形内容中提取文本的 IOcrConnector 实现。（继承自 [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)） |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # 区分大小写的替换
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
使用 `ExactPhraseRedaction` 的任务指南：

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 另请参阅
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
