---
title: "Класс RegexRedaction"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет текстовое редактирование, которое ищет и заменяет текст в документе, сопоставляя предоставленное регулярное выражение."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

Представляет текстовое редактирование, которое ищет и заменяет текст в документе, сопоставляя предоставленное регулярное выражение.

Узнать больше

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

Тип RegexRedaction раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | Инициализирует новый экземпляр RegexRedaction. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | Инициализирует новый экземпляр RegexRedaction. |

### Методы
| Метод | Описание |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | Применяет редактирование к заданному экземпляру формата. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### Свойства
| Свойство | Описание |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | Описание редактирования, содержащее его имя и параметры. |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Шаблон регулярного выражения, используемый для сопоставления. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Экземпляр [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) указывающий тип замены текста. (унаследовано от [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Реализация IOcrConnector, используемая для извлечения текста из графического контента. (унаследовано от [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # заменить текстом
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # заменить синим сплошным прямоугольником
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
Руководства задач, использующие `RegexRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
