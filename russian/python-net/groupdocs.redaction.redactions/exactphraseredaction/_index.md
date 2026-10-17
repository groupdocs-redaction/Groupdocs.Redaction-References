---
title: "ExactPhraseRedaction класс"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет текстовое редактирование, которое заменяет точную фразу в тексте документа, без учёта регистра по умолчанию."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

Представляет текстовое редактирование, которое заменяет точную фразу в тексте документа, без учёта регистра по умолчанию.

Узнать больше:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

Тип ExactPhraseRedaction раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | Инициализирует новый экземпляр ExactPhraseRedaction в режиме без учёта регистра. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | Инициализирует новый экземпляр ExactPhraseRedaction. |

### Методы
| Метод | Описание |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | Применяет редактирование к заданному экземпляру формата. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### Свойства
| Свойство | Описание |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | Описание редактирования, содержащее имя редактирования и параметры. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | Значение, указывающее, является ли поиск чувствительным к регистру. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | Флаг направления текста, указывающий, является ли текст справа налево. По умолчанию False. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | Строка для поиска и замены. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Экземпляр [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) указывающий тип замены текста. (унаследовано от [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Реализация IOcrConnector, используемая для извлечения текста из графического контента. (унаследовано от [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # замена с учётом регистра
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
Руководства задач, использующие `ExactPhraseRedaction`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
