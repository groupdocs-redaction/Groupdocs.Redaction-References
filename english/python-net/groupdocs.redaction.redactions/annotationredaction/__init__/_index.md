---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new AnnotationRedaction with a regex pattern and replacement text."
type: docs
url: /python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

Initializes a new AnnotationRedaction with a regex pattern and replacement text.

```python
def __init__(self, pattern, replacement):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pattern | `str` | Regular expression to match. |
| replacement | `str` | Textual replacement for matched text. |

### Example

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Redact the word "approved" in annotation texts
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

Initializes a new instance of [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/).

```python
def __init__(self, regex, replacement):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Regular expression to match. |
| replacement | `str` | Textual replacement for matched text. |

### Example

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Redact the word "approved" (case‑insensitive) and replace it with "[REVIEW]"
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### See Also
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
