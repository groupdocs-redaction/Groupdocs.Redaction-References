---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new DeleteAnnotationRedaction instance that deletes all annotations (matches everything)."
type: docs
url: /python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new DeleteAnnotationRedaction instance that deletes all annotations (matches everything).

```python
def __init__(self):
    ...
```

## __init__ {#pattern}

Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching the given regular expression.

```python
def __init__(self, pattern):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pattern | `str` | Regular expression. |

### Example

```python
    from groupdocs.redaction import Redactor
    from groupdocs.redaction.redactions import DeleteAnnotationRedaction

    with Redactor("document.pdf") as redactor:
        redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
        redactor.save()
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

# Delete annotations whose text matches the case‑insensitive pattern "internal"
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### See Also
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
