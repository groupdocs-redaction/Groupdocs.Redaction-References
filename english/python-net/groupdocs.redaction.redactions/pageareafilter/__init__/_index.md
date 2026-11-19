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
| top_left | `Point` | Top-left area coordinates. |
| size | `Size` | Area size. |

### Example

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.redaction.options.drawing import Point, Size

# Define the top-left corner and size of the redaction area
top_left = Point(0, 100)
area_size = Size(200, 150)

# Create the filter
filter = PageAreaFilter(top_left, area_size)
```

### See Also
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
