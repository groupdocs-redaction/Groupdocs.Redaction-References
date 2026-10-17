---
title: "метод replace_in_column"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Заменяет все совпадения заданной заменой в указанном столбце и листе."
type: docs
url: /ru/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

Заменяет все совпадения заданной заменой в указанном столбце и листе.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Регулярное выражение для поиска и замены. |
| replacement | `str` | Текстовая замена. |
| column | `int` | Индекс столбца, начиная с нуля. |
| sheet | `int` | Индекс листа, начиная с нуля. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

Заменяет все совпадения заданной заменой в указанном столбце на всех листах.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Регулярное выражение для поиска и замены. |
| replacement | `str` | Текстовая замена. |
| column | `int` | Индекс столбца, начиная с нуля. |

**Returns:** Replacement result.

### См. также
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
