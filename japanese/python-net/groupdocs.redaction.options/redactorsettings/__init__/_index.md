---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "RedactorSettings クラスの新しいインスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

RedactorSettings クラスの新しいインスタンスを初期化します。

```python
def __init__(self):
    ...
```

### 例

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

指定された ILogger インスタンスを使用して新しい RedactorSettings インスタンスを初期化します。

```python
def __init__(self, logger):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| logger | `ILogger` | `ILogger` インターフェイスを実装するクラスのインスタンスです。 |

## __init__ {#callback}

指定された IRedactionCallback インスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。

```python
def __init__(self, callback):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| callback | `IRedactionCallback` | IRedactionCallback インターフェイスを実装するクラスのインスタンスです。 |

### 例

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

指定された IOcrConnector を使用して新しい RedactorSettings インスタンスを初期化します。

```python
def __init__(self, ocr_connector):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | IOcrConnector インターフェイスの有効な実装です。 |

## __init__ {#logger-callback}

指定されたロガーとコールバックを使用して新しい RedactorSettings インスタンスを初期化します。

```python
def __init__(self, logger, callback):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| logger | `ILogger` | ILogger インターフェイスを実装するクラスのインスタンスです。 |
| callback | `IRedactionCallback` | IRedactionCallback インターフェイスを実装するクラスのインスタンスです。 |

### 例

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

指定された ILogger、IRedactionCallback、IOcrConnector のインスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| logger | `ILogger` | `ILogger` インターフェイスを実装するクラスのインスタンスです。 |
| callback | `IRedactionCallback` | `IRedactionCallback` インターフェイスを実装するクラスのインスタンスです。 |
| ocr_connector | `IOcrConnector` | `IOcrConnector` インターフェイス実装のインスタンスです。`None` にすることもできます。 |

### 例

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### 関連項目
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
