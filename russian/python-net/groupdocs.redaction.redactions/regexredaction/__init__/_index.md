---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр RegexRedaction."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

Инициализирует новый экземпляр RegexRedaction.

```python
def __init__(self, pattern, options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| pattern | `str` | Регулярное выражение для поиска и замены. |
| options | `ReplacementOptions` | Replacement options (textual, color). |

### Пример

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

Инициализирует новый экземпляр RegexRedaction.

```python
def __init__(self, regex, options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Регулярное выражение для поиска и замены. |
| options | `ReplacementOptions` | Replacement options (textual, color). |

### Пример

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### См. также
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
