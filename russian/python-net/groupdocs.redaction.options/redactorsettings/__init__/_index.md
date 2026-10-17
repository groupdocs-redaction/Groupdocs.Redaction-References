---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр класса RedactorSettings."
type: docs
url: /ru/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

Инициализирует новый экземпляр класса RedactorSettings.

```python
def __init__(self):
    ...
```

### Пример

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

Инициализирует новый экземпляр RedactorSettings с заданным экземпляром ILogger.

```python
def __init__(self, logger):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| logger | `ILogger` | Экземпляр класса, реализующего интерфейс `ILogger`. |

## __init__ {#callback}

Инициализирует новый экземпляр класса RedactorSettings с заданным экземпляром IRedactionCallback.

```python
def __init__(self, callback):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| callback | `IRedactionCallback` | Экземпляр класса, реализующего интерфейс IRedactionCallback. |

### Пример

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

Инициализирует новый экземпляр RedactorSettings с указанным IOcrConnector.

```python
def __init__(self, ocr_connector):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | Корректная реализация интерфейса IOcrConnector. |

## __init__ {#logger-callback}

Инициализирует новый экземпляр RedactorSettings с указанным логгером и обратным вызовом.

```python
def __init__(self, logger, callback):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| logger | `ILogger` | Экземпляр класса, реализующего интерфейс ILogger. |
| callback | `IRedactionCallback` | Экземпляр класса, реализующего интерфейс IRedactionCallback. |

### Пример

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

Инициализирует новый экземпляр класса RedactorSettings с заданными экземплярами ILogger, IRedactionCallback и IOcrConnector.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| logger | `ILogger` | Экземпляр класса, реализующего интерфейс `ILogger`. |
| callback | `IRedactionCallback` | Экземпляр класса, реализующего интерфейс `IRedactionCallback`. |
| ocr_connector | `IOcrConnector` | Экземпляр реализации интерфейса `IOcrConnector`. Может быть `None`. |

### Пример

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### См. также
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
