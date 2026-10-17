---
title: "Класс DeleteAnnotationRedaction"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет текстовое редактирование, которое удаляет аннотации, если текст соответствует заданному регулярному выражению (опционально удаляет все аннотации)."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

Представляет текстовое редактирование, которое удаляет аннотации, если текст соответствует заданному регулярному выражению (опционально удаляет все аннотации).

Узнать больше

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

Тип DeleteAnnotationRedaction раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | Инициализирует новый экземпляр класса DeleteAnnotationRedaction с настройками для удаления всех аннотаций (соответствующих всему). |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | Инициализирует новый экземпляр класса DeleteAnnotationRedaction, удаляя аннотации, соответствующие заданному выражению. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | Инициализирует новый экземпляр класса DeleteAnnotationRedaction, удаляя аннотации, соответствующие заданному выражению. |

### Методы
| Метод | Описание |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | Применяет редактирование к заданному экземпляру формата. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### Свойства
| Свойство | Описание |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | Описание редактирования, содержащее имя редактирования и параметры. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | Регулярное выражение для сопоставления. |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # Удалить аннотации, содержащие слово "internal" (без учёта регистра)
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
Руководства задач, использующие `DeleteAnnotationRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
