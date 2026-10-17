---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый ImageAreaRedaction для редактирования конкретной прямоугольной области."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

Инициализирует новый ImageAreaRedaction для редактирования конкретной прямоугольной области.

```python
def __init__(self, top_left, options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Координаты области в левом верхнем углу. |
| options | `RegionReplacementOptions` | Размер и цвет области. |

### Пример

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# Определите левый верхний угол области для редактирования
top_left = Point(385, 485)
# Определите размер и цвет области редактирования
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# Создайте объект редактирования
redaction = ImageAreaRedaction(top_left, region_options)
```

### См. также
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
