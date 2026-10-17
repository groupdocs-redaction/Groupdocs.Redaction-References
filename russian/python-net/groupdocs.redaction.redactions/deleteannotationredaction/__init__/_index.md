---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр класса DeleteAnnotationRedaction с настройками для удаления всех аннотаций (соответствующих всему)."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

Инициализирует новый экземпляр класса DeleteAnnotationRedaction с настройками для удаления всех аннотаций (соответствующих всему).

```python
def __init__(self):
    ...
```

### Пример

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Удалить все аннотации
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

Инициализирует новый экземпляр класса DeleteAnnotationRedaction, удаляя аннотации, соответствующие заданному выражению.

```python
def __init__(self, pattern):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| pattern | `str` | Регулярное выражение. |

### Пример

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Удалить аннотации, содержащие слово "internal" (без учёта регистра)
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

Инициализирует новый экземпляр класса DeleteAnnotationRedaction, удаляя аннотации, соответствующие заданному выражению.

```python
def __init__(self, regex):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Регулярное выражение. |

### Пример

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Удалить аннотации, содержимое которых соответствует регулярному выражению (без учёта регистра)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### См. также
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
