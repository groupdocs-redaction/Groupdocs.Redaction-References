---
title: PageRangeFilter class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a redaction filter that sets the page range inside a document to apply redaction."
type: docs
url: /python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

Represents a redaction filter that sets the page range inside a document to apply redaction.

- More details about applying redactions: https://docs.groupdocs.com/redaction/python-net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/python-net/use-pdf-redaction-filters/

The PageRangeFilter type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | Initializes a new instance of PageRangeFilter. |

### Properties
| Property | Description |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | The number of pages to remove. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | The start position index (0-based). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | The seek reference position, either the beginning or the end of a document. |

### Example

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# Create a filter for the last page (origin END, offset 0, count 1)
filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)
```

### Guides
Task guides that use `PageRangeFilter`:

* [Use PageAreaRedaction](/redaction/python-net/guides/use-page-area-redaction/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
