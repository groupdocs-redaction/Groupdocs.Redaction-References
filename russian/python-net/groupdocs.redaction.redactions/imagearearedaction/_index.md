---
title: "ImageAreaRedaction класс"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет редактирование, которое размещает цветной прямоугольник в заданной области изображения документа."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

Представляет редактирование, которое размещает цветной прямоугольник в заданной области изображения документа.

Узнать больше:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Тип ImageAreaRedaction раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | Инициализирует новый ImageAreaRedaction для редактирования конкретной прямоугольной области. |

### Методы
| Метод | Описание |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | Применяет редактирование к заданному экземпляру формата. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to_document_format_instance/) |  |

### Свойства
| Свойство | Описание |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | Описание редактирования, содержащее его имя и параметры. |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | Параметры RegionReplacementOptions с параметрами цвета и области. |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | Позиция верхнего левого угла области для удаления. |

### Пример

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

point = Point(516, 311)
size = Size(170, 35)
color = Color.from_argb(255, 0, 0, 255)  # blue
options = RegionReplacementOptions(color, size)
redaction = ImageAreaRedaction(point, options)

with Redactor("D:\\test.jpg") as redactor:
    result = redactor.apply(redaction)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Руководства задач, использующие `ImageAreaRedaction`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
