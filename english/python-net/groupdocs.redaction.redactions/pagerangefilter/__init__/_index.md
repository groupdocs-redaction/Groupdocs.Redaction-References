---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance of PageRangeFilter."
type: docs
url: /python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

Initializes a new instance of PageRangeFilter.

```python
def __init__(self, origin, index, count):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Seek reference position, the beginning or the end of a document. |
| index | `int` | Start position index (0-based). |
| count | `int` | Count of pages to remove. |

### Example

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

filters = [
    PageRangeFilter(PageSeekOrigin.END, 0, 1),
    # add other filters as needed
]
```

### See Also
* class [`PageRangeFilter`](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/)
