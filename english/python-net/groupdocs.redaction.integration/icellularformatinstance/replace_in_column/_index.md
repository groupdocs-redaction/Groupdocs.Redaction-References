---
title: replace_in_column method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Replaces all matches with a given replacement in the specified column and worksheet."
type: docs
url: /python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

Replaces all matches with a given replacement in the specified column and worksheet.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace. |
| replacement | `str` | Textual replacement. |
| column | `int` | Zero-based column index. |
| sheet | `int` | Zero-based worksheet index. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

Replaces all matches with a given replacement in the specified column on all worksheets.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace. |
| replacement | `str` | Textual replacement. |
| column | `int` | Zero-based column index. |

**Returns:** Replacement result.

### See Also
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
