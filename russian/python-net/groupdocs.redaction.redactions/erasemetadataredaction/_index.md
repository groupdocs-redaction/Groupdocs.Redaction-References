---
title: "Класс EraseMetadataRedaction"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет редактирование метаданных, которое стирает все метаданные или метаданные, соответствующие определённым MetadataFilters, из документа."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

Представляет редактирование метаданных, которое стирает все метаданные или метаданные, соответствующие определённым MetadataFilters, из документа.

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

Тип EraseMetadataRedaction раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | Инициализирует новый экземпляр класса EraseMetadataRedaction, удаляя все метаданные. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | Инициализирует новый экземпляр EraseMetadataRedaction, удаляя метаданные, соответствующие указанным `MetadataFilters`. |

### Методы
| Метод | Описание |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Применяет редактирование к заданному экземпляру формата. (наследовано от [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (наследовано от [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Свойства
| Свойство | Описание |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | Описание редактирования и его параметров. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Фильтр, используемый для выбора всех или конкретных метаданных, таких как Author или Company. (наследовано от [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Удалить все метаданные
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Удалить только поле автора
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
Руководства задач, использующие `EraseMetadataRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
