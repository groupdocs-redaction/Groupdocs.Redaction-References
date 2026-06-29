---
title: PageRangeFilter class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents redaction filter, setting page range inside a document to apply redaction."
type: docs
url: /python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

Represents redaction filter, setting page range inside a document to apply redaction.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

The PageRangeFilter type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | Initializes a new RemovePageRedaction. |

### Properties
| Property | Description |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | The count of pages to remove. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | The start position index (0-based). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | The seek reference position, either the beginning or the end of a document. |

### Example

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# Define a filter that targets the last page and the one before it
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# The filter can be combined with other filters, e.g., PageAreaFilter,
# and passed to ReplacementOptions.Filters when configuring a redaction.
```

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
