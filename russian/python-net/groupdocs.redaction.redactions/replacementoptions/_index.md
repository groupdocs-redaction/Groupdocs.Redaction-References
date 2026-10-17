---
title: "Класс ReplacementOptions"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет параметры для замены найденного текста."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

Представляет параметры для замены найденного текста.

Узнать больше

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Тип ReplacementOptions раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | Инициализирует новый экземпляр ReplacementOptions с указанным текстом замены. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | Инициализирует новый экземпляр класса ReplacementOptions с цветным прямоугольником в качестве опции. |

### Свойства
| Свойство | Описание |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | Действие замены: нарисовать рамку или заменить текст. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | Цвет для опции `ReplacementType.draw_box` (в остальных случаях игнорируется). |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | Пользовательский обработчик редактирования, позволяющий пользователям определять собственную логику редактирования. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | Массив фильтров, применяемых к этому редактированию. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | Текстовое значение замены. |

### Пример

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Заменить найденный текст на заполнитель "[X]"
repl_opt = ReplacementOptions("[X]")
```

### Guides
Руководства задач, использующие `ReplacementOptions`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
