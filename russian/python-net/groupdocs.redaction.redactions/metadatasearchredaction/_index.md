---
title: "Класс MetadataSearchRedaction"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет редактирование метаданных, которое ищет и редактирует метаданные с помощью регулярных выражений, сопоставляя ключи и/или значения."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

Представляет редактирование метаданных, которое ищет и редактирует метаданные с помощью регулярных выражений, сопоставляя ключи и/или значения.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

Тип MetadataSearchRedaction раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | Инициализирует новый экземпляр класса MetadataSearchRedaction, используя значение для сопоставления скрываемых элементов. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | Инициализирует новый экземпляр MetadataSearchRedaction, используя имя элемента и значение для сопоставления скрываемых элементов. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | Инициализирует новый экземпляр класса MetadataSearchRedaction, используя значение для сопоставления скрываемых элементов. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | Инициализирует новый экземпляр MetadataSearchRedaction, используя имя элемента и значение для сопоставления скрываемых элементов. |

### Методы
| Метод | Описание |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Применяет редактирование к заданному экземпляру формата. (наследовано от [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (наследовано от [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Свойства
| Свойство | Описание |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | Описание редактирования, содержащее его имя и параметры. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | Регулярное выражение для сопоставления имени (ключа) элемента метаданных. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | Текстовое значение замены. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | Регулярное выражение для сопоставления текстового значения элемента метаданных. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Фильтр, используемый для выбора всех или конкретных метаданных, таких как Author или Company. (наследовано от [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Скрыть любое значение метаданных, соответствующее шаблону
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
Руководства задач, использующие `MetadataSearchRedaction`:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
