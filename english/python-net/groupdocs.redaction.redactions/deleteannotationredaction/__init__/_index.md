---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance of DeleteAnnotationRedaction class, with settings to delete all annotations (matching everything)."
type: docs
url: /python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of DeleteAnnotationRedaction class, with settings to delete all annotations (matching everything).

```python
def __init__(self):
    ...
```

### Example

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Delete all annotations
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching given expression.

```python
def __init__(self, pattern):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pattern | `str` | Regular expression. |

### Example

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Delete annotations containing the word "internal" (case‑insensitive)
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching given expression.

```python
def __init__(self, regex):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Regular expression. |

### Example

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Delete annotations whose content matches the regex (case‑insensitive)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### See Also
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
