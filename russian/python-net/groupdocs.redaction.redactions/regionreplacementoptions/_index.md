---
title: "Класс RegionReplacementOptions"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет параметры цвета и области для замены региона изображения."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

Представляет параметры цвета и области для замены региона изображения.

Узнать больше:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Тип RegionReplacementOptions раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | Инициализирует новый экземпляр RegionReplacementOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | Инициализирует новый экземпляр класса RegionReplacementOptions, размер которого соответствует заданному тексту. |

### Свойства
| Свойство | Описание |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | Цвет, используемый для заполнения редактируемой области. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | Ширина и высота прямоугольника. |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # Определите позицию верхнего‑левого угла области для замены
    point = Point(516, 311)
    # Определите размер области для замены
    size = Size(170, 35)
    # Используйте сплошной чёрный прямоугольник в качестве замены
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Руководства задач, использующие `RegionReplacementOptions`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
