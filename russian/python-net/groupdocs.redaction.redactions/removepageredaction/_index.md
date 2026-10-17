---
title: "RemovePageRedaction класс"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет редактирование, которое удаляет страницу (слайд, лист, и т.д.) из документа."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

Представляет редактирование, которое удаляет страницу (слайд, лист, и т.д.) из документа.

Узнать больше
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

Тип RemovePageRedaction раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | Инициализирует новый RemovePageRedaction. |

### Методы
| Метод | Описание |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | Применяет редактирование к заданному экземпляру формата. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### Свойства
| Свойство | Описание |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | Количество страниц для удаления. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | Индекс начальной позиции (нумерация с нуля). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | Позиция ссылки поиска, либо начало, либо конец документа. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | Описание редактирования, содержащее его имя и параметры. (унаследовано от [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Удалить 1 страницу, считая от конца документа
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # Применить редактирование
        result = redactor.apply(rem_opt)

        # Сохраните отредактированный документ
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
Руководства задач, использующие `RemovePageRedaction`:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
