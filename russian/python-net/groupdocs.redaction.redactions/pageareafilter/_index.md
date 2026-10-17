---
title: "Класс PageAreaFilter"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет фильтр редактирования, задающий область внутри страницы документа для применения редактирования."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

Представляет фильтр редактирования, задающий область внутри страницы документа для применения редактирования.

Узнать больше

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Тип PageAreaFilter раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | Инициализирует новый PageAreaFilter для редактирования конкретной области. |

### Свойства
| Свойство | Описание |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | Прямоугольник (позиция верхнего левого угла и размер области) на странице. |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
