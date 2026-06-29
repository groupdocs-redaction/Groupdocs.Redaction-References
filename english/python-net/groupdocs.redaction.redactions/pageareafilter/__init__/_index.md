---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new PageAreaFilter for redacting a specific area."
type: docs
url: /python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

Initializes a new PageAreaFilter for redacting a specific area.

```python
def __init__(self, top_left, size):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Top-left area coordinates. |
| size | `System.Drawing.Size` | Area size and color. |

### Example

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### See Also
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
