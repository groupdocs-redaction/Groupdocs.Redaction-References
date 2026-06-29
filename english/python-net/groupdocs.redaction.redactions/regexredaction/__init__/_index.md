---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance of RegexRedaction."
type: docs
url: /python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

Initializes a new instance of RegexRedaction.

```python
def __init__(self, pattern, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pattern | `str` | Regular expression to search and replace. |
| options | `ReplacementOptions` | Replacement options (textual, color). |

### Example

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

Initializes a new RegexRedaction instance.

```python
def __init__(self, regex, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace. |
| options | `ReplacementOptions` | Replacement options (textual, color). |

### Example

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### See Also
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
