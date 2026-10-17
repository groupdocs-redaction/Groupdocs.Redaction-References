---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化 RedactorSettings 类的新实例。"
type: docs
url: /zh/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

初始化 RedactorSettings 类的新实例。

```python
def __init__(self):
    ...
```

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

## __init__ {#logger}

使用给定的 ILogger 实例初始化一个新的 RedactorSettings 实例。

```python
def __init__(self, logger):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| logger | `ILogger` | 实现 `ILogger` 接口的类的实例。 |

## __init__ {#callback}

使用给定的 IRedactionCallback 实例初始化 RedactorSettings 类的新实例。

```python
def __init__(self, callback):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| callback | `IRedactionCallback` | 实现 IRedactionCallback 接口的类的实例。 |

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

## __init__ {#ocr_connector}

使用指定的 IOcrConnector 初始化一个新的 RedactorSettings 实例。

```python
def __init__(self, ocr_connector):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | IOcrConnector 接口的有效实现。 |

## __init__ {#logger-callback}

使用指定的日志记录器和回调初始化一个新的 RedactorSettings 实例。

```python
def __init__(self, logger, callback):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| logger | `ILogger` | 实现 ILogger 接口的类的实例。 |
| callback | `IRedactionCallback` | 实现 IRedactionCallback 接口的类的实例。 |

### 示例

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

使用给定的 ILogger、IRedactionCallback 和 IOcrConnector 实例初始化 RedactorSettings 类的新实例。

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| logger | `ILogger` | 实现 `ILogger` 接口的类的实例。 |
| callback | `IRedactionCallback` | 实现 `IRedactionCallback` 接口的类的实例。 |
| ocr_connector | `IOcrConnector` | `IOcrConnector` 接口实现的实例。可以为 `None`。 |

### 示例

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### 另请参阅
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
