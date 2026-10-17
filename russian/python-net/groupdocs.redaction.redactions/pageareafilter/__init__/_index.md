---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый PageAreaFilter для редактирования конкретной области."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

Инициализирует новый PageAreaFilter для редактирования конкретной области.

```python
def __init__(self, top_left, size):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Координаты области в левом верхнем углу. |
| size | `System.Drawing.Size` | Размер и цвет области. |

### Пример

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### См. также
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
