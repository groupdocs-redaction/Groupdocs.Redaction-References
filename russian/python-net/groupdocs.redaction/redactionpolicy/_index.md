---
title: "RedactionPolicy класс"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет политику очистки, содержащую набор конкретных редактирований для применения."
type: docs
url: /ru/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

Представляет политику очистки, содержащую набор конкретных редактирований для применения.

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

Тип RedactionPolicy раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | Инициализирует новый экземпляр RedactionPolicy. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | Инициализирует новый RedactionPolicy со специфическим списком редактирований. |

### Методы
| Метод | Описание |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | Загружает RedactionPolicy из XML‑файла. |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | Загружает экземпляр RedactionPolicy из потока, содержащего XML‑конфигурацию. |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | Сохраняет политику редактирования в файл. |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | Сохраняет политику редактирования в поток. |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### Свойства
| Свойство | Описание |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | Список полностью сконфигурированных классов, наследованных от [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/). |

### Пример

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# Создайте переиспользуемую политику в памяти
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# Примените политику к документу
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
Руководства задач, использующие `RedactionPolicy`:

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### См. также
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
