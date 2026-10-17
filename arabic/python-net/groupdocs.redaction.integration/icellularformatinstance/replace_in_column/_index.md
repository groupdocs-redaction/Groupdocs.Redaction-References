---
title: "طريقة replace_in_column"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يستبدل جميع التطابقات بالبديل المحدد في العمود والورقة المحددين."
type: docs
url: /ar/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

يستبدل جميع التطابقات بالبديل المحدد في العمود والورقة المحددين.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | تعبير نمطي للبحث والاستبدال. |
| replacement | `str` | استبدال نصي. |
| column | `int` | فهرس العمود يبدأ من الصفر. |
| sheet | `int` | فهرس ورقة العمل يبدأ من الصفر. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

يستبدل جميع التطابقات بالبديل المحدد في العمود المحدد على جميع أوراق العمل.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | تعبير نمطي للبحث والاستبدال. |
| replacement | `str` | استبدال نصي. |
| column | `int` | فهرس العمود يبدأ من الصفر. |

**Returns:** Replacement result.

### انظر أيضًا
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
