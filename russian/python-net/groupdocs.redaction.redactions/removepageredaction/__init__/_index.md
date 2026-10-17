---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый RemovePageRedaction."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

Инициализирует новый RemovePageRedaction.

```python
def __init__(self, origin, index, count):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Ищите позицию ссылки, начало или конец документа. |
| index | `int` | Индекс начальной позиции (нумерация с нуля). |
| count | `int` | Количество страниц для удаления. |

### Пример

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Удалить 3 страницы, начиная со второй страницы (индекс с нуля 1)
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### См. также
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
