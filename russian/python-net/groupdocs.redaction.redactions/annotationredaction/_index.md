---
title: "Класс AnnotationRedaction"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет редактирование, которое заменяет текст аннотации (комментарии и т.п.), соответствующий заданному регулярному выражению."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

Представляет редактирование, которое заменяет текст аннотации (комментарии и т.п.), соответствующий заданному регулярному выражению.

Узнать больше

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

Тип AnnotationRedaction раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | Инициализирует новый AnnotationRedaction с шаблоном regex и текстом замены. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | Инициализирует новый экземпляр [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/). |

### Методы
| Метод | Описание |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | Применяет редактирование к заданному экземпляру формата. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### Свойства
| Свойство | Описание |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | Описание редактирования, описывающее редактирование и его параметры. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | Регулярное выражение для сопоставления. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | Текстовая замена найденного текста. |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
Руководства задач, использующие `AnnotationRedaction`:

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
