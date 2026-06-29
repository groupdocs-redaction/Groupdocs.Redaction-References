---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance of ReplacementOptions with the specified replacement text."
type: docs
url: /python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

Initializes a new instance of ReplacementOptions with the specified replacement text.

```python
def __init__(self, replacement):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| replacement | `str` | Textual replacement. |

### Example

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Replace matched text with "[REDACTED]"
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

Initializes a new instance of ReplacementOptions class with colored rectangle as an option.

```python
def __init__(self, color):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| color | `System.Drawing.Color` | Rectangle color. |

### See Also
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
