---
title: "метод remove_pages"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Удаляет одну или несколько страниц в зависимости от их начальной позиции, смещения и количества."
type: docs
url: /ru/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

Удаляет одну или несколько страниц в зависимости от их начальной позиции, смещения и количества.

```python
def remove_pages(self, origin, index, count):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Позиция начала поиска, начало или конец документа. |
| index | `int` | Индекс начальной позиции (нумерация с нуля). |
| count | `int` | Количество страниц для удаления. |

**Returns:** Pages removal redaction result.

### См. также
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
