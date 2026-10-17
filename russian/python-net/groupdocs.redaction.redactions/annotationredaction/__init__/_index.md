---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый AnnotationRedaction с шаблоном regex и текстом замены."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

Инициализирует новый AnnotationRedaction с шаблоном regex и текстом замены.

```python
def __init__(self, pattern, replacement):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| pattern | `str` | Регулярное выражение для сопоставления. |
| replacement | `str` | Текстовая замена найденного текста. |

### Пример

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Замаскировать слово "approved" в аннотационных текстах
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

Инициализирует новый экземпляр [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/).

```python
def __init__(self, regex, replacement):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Регулярное выражение для сопоставления. |
| replacement | `str` | Текстовая замена найденного текста. |

### Пример

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Замаскировать слово "approved" (без учёта регистра) и заменить его на "[REVIEW]"
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### См. также
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
