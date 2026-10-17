---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый CellColumnRedaction."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

Инициализирует новый CellColumnRedaction.

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| filter | `CellFilter` | Фильтр столбцов и листов. |
| reg_ex | `System.Text.RegularExpressions.Regex` | Регулярное выражение для поиска и замены. |
| options | `ReplacementOptions` | Параметры замены. |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("spreadsheet.xlsx") as redactor:
    redactor.apply(
        CellColumnRedaction(
            CellFilter(worksheet="Sheet1", column=2),
            r"\bsecret\b",
            ReplacementOptions(Color.BLACK)
        )
    )
    redactor.save()
```

### См. также
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
