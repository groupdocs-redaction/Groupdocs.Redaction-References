---
title: redact_annotation method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Replaces the matching text in all annotations within the document."
type: docs
url: /python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation/
is_root: false
weight: 1020
---


## redact_annotation {#regular_expression-replacement}

Replaces the matching text in all annotations within the document.

```python
def redact_annotation(self, regular_expression, replacement):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace. |
| replacement | `str` | Textual replacement. |

**Returns:** Replacement result.

### Aliases

These names call `redact_annotation` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `redact_annotation_regex` | `redact_annotation_regex(regular_expression, replacement)` |
| `redact_annotation_file` | `redact_annotation_file(regular_expression, replacement)` |
| `redact_annotation_string` | `redact_annotation_string(regular_expression, replacement)` |

### See Also
* class [`IAnnotatedDocument`](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/)
