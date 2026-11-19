---
title: PageAreaFilter class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents redaction filter, setting an area within a page of a document to apply redaction."
type: docs
url: /python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

Represents redaction filter, setting an area within a page of a document to apply redaction.

Learn more

- More details about applying redactions: https://docs.groupdocs.com/redaction/python-net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/python-net/use-pdf-redaction-filters/

The PageAreaFilter type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | Initializes a new PageAreaFilter for redacting a specific area. |

### Properties
| Property | Description |
| :- | :- |
| [area_rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/area_rectangle/) | The rectangle (top-left position and size of the area) on a page. |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | The rectangle (top-left position and size of the area) on a page. |

### Example

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.redaction.options.drawing import Point, Size

# Define the top‑left corner of the area
origin = Point(0, 100)

# Define the size of the area
area_size = Size(200, 300)

# Create a filter that limits redaction to the specified rectangle
filter = PageAreaFilter(origin, area_size)
```

### Guides
Task guides that use `PageAreaFilter`:

* [Use PageAreaRedaction](/redaction/python-net/guides/use-page-area-redaction/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
