---
title: "redact_annotation 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "替换文档中所有注释中匹配的文本。"
type: docs
url: /zh/python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation/
is_root: false
weight: 1030
---


## redact_annotation {#regular_expression-replacement}

替换文档中所有注释中匹配的文本。

```python
def redact_annotation(self, regular_expression, replacement):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | 用于搜索和替换的正则表达式。 |
| replacement | `str` | 文本替换。 |

**Returns:** Replacement result.

### 另请参阅
* class [`IAnnotatedDocument`](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/)
