---
title: "RedactorSettings 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示编辑设置，允许自定义编辑过程。"
type: docs
url: /zh/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

表示编辑设置，允许自定义编辑过程。

了解更多

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

RedactorSettings 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | 初始化 RedactorSettings 类的新实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | 使用给定的 ILogger 实例初始化一个新的 RedactorSettings 实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | 使用给定的 IRedactionCallback 实例初始化 RedactorSettings 类的新实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | 使用指定的 IOcrConnector 初始化一个新的 RedactorSettings 实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | 使用指定的日志记录器和回调初始化一个新的 RedactorSettings 实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | 使用给定的 ILogger、IRedactionCallback 和 IOcrConnector 实例初始化 RedactorSettings 类的新实例。 |

### 属性
| 属性 | 描述 |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | 用于记录事件和错误的日志记录器。必须是实现 [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/) 的类的实例。 |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | 实现 [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/) 的 OCR 连接器实例。 |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | 用于评估每个脱敏描述的脱敏回调。 |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import LoadOptions, RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", LoadOptions(), RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

### 另请参阅
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
