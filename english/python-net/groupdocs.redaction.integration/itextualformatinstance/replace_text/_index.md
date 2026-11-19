---
title: replace_text method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Replaces all matches of the regular expression with a given replacement."
type: docs
url: /python-net/groupdocs.redaction.integration/itextualformatinstance/replace_text/
is_root: false
weight: 1010
---


## replace_text {#regular_expression-options}

Replaces all matches of the regular expression with a given replacement.

```python
def replace_text(self, regular_expression, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace. |
| options | `ReplacementOptions` | Allows setting textual replacement or color for the redaction block. |

**Returns:** Text replacement result.

### Aliases

These names call `replace_text` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `replace_text_regex` | `replace_text_regex(regular_expression, options)` |

### See Also
* class [`ITextualFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/itextualformatinstance/)
