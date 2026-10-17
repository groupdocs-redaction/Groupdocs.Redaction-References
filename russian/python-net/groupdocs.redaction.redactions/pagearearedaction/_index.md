---
title: "Класс PageAreaRedaction"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет сложное текстовое редактирование, которое влияет на текст, изображения и аннотации в области страницы."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

Представляет сложное текстовое редактирование, которое влияет на текст, изображения и аннотации в области страницы.

Узнать больше

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

Тип PageAreaRedaction раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | Инициализирует новый экземпляр PageAreaRedaction. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | Инициализирует новый PageAreaRedaction. |

### Методы
| Метод | Описание |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | Применяет редактирование к заданному экземпляру формата. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### Свойства
| Свойство | Описание |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | Параметры RegionReplacementOptions с параметрами цвета и области. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Экземпляр [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) указывающий тип замены текста. (унаследовано от [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | Описание редактирования, содержащее его имя и параметры. (унаследовано от [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Реализация IOcrConnector, используемая для извлечения текста из графического контента. (унаследовано от [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Регулярное выражение, используемое для сопоставления. (унаследовано от [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(
            r"\d{3}-\d{2}-\d{4}",
            ReplacementOptions("[SSN]"),
            RegionReplacementOptions(Color.BLACK, Size(120, 20))
        )
    )
    redactor.save()
```

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
