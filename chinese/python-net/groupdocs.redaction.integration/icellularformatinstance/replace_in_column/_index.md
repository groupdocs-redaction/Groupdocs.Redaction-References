---
title: "replace_in_column 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "在指定的列和工作表中，用给定的替换内容替换所有匹配项。"
type: docs
url: /zh/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

在指定的列和工作表中，用给定的替换内容替换所有匹配项。

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | 用于搜索和替换的正则表达式。 |
| replacement | `str` | 文本替换。 |
| column | `int` | 从零开始的列索引。 |
| sheet | `int` | 从零开始的工作表索引。 |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

在所有工作表的指定列中，用给定的替换内容替换所有匹配项。

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | 用于搜索和替换的正则表达式。 |
| replacement | `str` | 文本替换。 |
| column | `int` | 从零开始的列索引。 |

**Returns:** Replacement result.

### 另请参阅
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
