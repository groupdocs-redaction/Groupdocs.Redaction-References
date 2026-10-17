---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр ExactPhraseRedaction в режиме без учёта регистра."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

Инициализирует новый экземпляр ExactPhraseRedaction в режиме без учёта регистра.

```python
def __init__(self, search_phrase, options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| search_phrase | `str` | Строка для поиска и замены. |
| options | `ReplacementOptions` | Replacement options (textual, color). |

### Пример

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Заменить вхождения "John Doe" на "[CUSTOMER]" (без учёта регистра)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

Инициализирует новый экземпляр ExactPhraseRedaction.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| search_phrase | `str` | Строка для поиска и замены. |
| is_case_sensitive | `bool` | True, если требуется поиск с учётом регистра. |
| options | `ReplacementOptions` | Replacement options (textual, color). |

### Пример

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Редактирование точной фразы без учёта регистра
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# Редактирование точной фразы с учётом регистра
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### См. также
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
