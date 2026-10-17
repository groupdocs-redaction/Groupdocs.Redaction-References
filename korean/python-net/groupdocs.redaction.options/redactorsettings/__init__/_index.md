---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "RedactorSettings 클래스의 새 인스턴스를 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

RedactorSettings 클래스의 새 인스턴스를 초기화합니다.

```python
def __init__(self):
    ...
```

### 예제

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

주어진 ILogger 인스턴스를 사용하여 새 RedactorSettings 인스턴스를 초기화합니다.

```python
def __init__(self, logger):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| logger | `ILogger` | `ILogger` 인터페이스를 구현하는 클래스의 인스턴스. |

## __init__ {#callback}

주어진 IRedactionCallback 인스턴스를 사용하여 RedactorSettings 클래스의 새 인스턴스를 초기화합니다.

```python
def __init__(self, callback):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| callback | `IRedactionCallback` | IRedactionCallback 인터페이스를 구현하는 클래스의 인스턴스. |

### 예제

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

지정된 IOcrConnector를 사용하여 새 RedactorSettings 인스턴스를 초기화합니다.

```python
def __init__(self, ocr_connector):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | IOcrConnector 인터페이스의 유효한 구현. |

## __init__ {#logger-callback}

지정된 로거와 콜백을 사용하여 새 RedactorSettings 인스턴스를 초기화합니다.

```python
def __init__(self, logger, callback):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| logger | `ILogger` | ILogger 인터페이스를 구현하는 클래스의 인스턴스. |
| callback | `IRedactionCallback` | IRedactionCallback 인터페이스를 구현하는 클래스의 인스턴스. |

### 예제

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

주어진 ILogger, IRedactionCallback 및 IOcrConnector 인스턴스를 사용하여 RedactorSettings 클래스의 새 인스턴스를 초기화합니다.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| logger | `ILogger` | `ILogger` 인터페이스를 구현하는 클래스의 인스턴스. |
| callback | `IRedactionCallback` | `IRedactionCallback` 인터페이스를 구현하는 클래스의 인스턴스. |
| ocr_connector | `IOcrConnector` | `IOcrConnector` 인터페이스 구현의 인스턴스입니다. `None`일 수 있습니다. |

### 예제

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### 또 보기
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
