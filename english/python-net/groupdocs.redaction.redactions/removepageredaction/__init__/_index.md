---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new RemovePageRedaction."
type: docs
url: /python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

Initializes a new RemovePageRedaction.

```python
def __init__(self, origin, index, count):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Seek reference position, the beginning or the end of a document. |
| index | `int` | Start position index (0‑based). |
| count | `int` | Count of pages to remove. |

### Example

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Remove 3 pages starting from the second page (zero‑based index 1)
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### See Also
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
