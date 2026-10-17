---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр ReplacementOptions с указанным текстом замены."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

Инициализирует новый экземпляр ReplacementOptions с указанным текстом замены.

```python
def __init__(self, replacement):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| replacement | `str` | Текстовая замена. |

### Пример

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Заменить найденный текст на "[REDACTED]"
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

Инициализирует новый экземпляр класса ReplacementOptions с цветным прямоугольником в качестве опции.

```python
def __init__(self, color):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| color | `System.Drawing.Color` | Цвет прямоугольника. |

### См. также
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
