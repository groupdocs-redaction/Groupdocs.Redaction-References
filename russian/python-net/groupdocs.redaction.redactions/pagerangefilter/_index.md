---
title: "Класс PageRangeFilter"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет фильтр редактирования, задающий диапазон страниц внутри документа для применения редактирования."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

Представляет фильтр редактирования, задающий диапазон страниц внутри документа для применения редактирования.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

Тип PageRangeFilter раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | Инициализирует новый RemovePageRedaction. |

### Свойства
| Свойство | Описание |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | Количество страниц для удаления. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | Индекс начальной позиции (нумерация с нуля). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | Позиция ссылки поиска, либо начало, либо конец документа. |

### Пример

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# Определите фильтр, который нацелен на последнюю страницу и предшествующую ей.
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# Фильтр можно комбинировать с другими фильтрами, например, PageAreaFilter,
# и передавать в ReplacementOptions.Filters при настройке редактирования.
```

### См. также
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
