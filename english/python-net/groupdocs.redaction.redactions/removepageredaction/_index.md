---
title: RemovePageRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a redaction that removes a page (slide, worksheet, etc.) from a document."
type: docs
url: /python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

Represents a redaction that removes a page (slide, worksheet, etc.) from a document.

Learn more
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

The RemovePageRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | Initializes a new RemovePageRedaction. |

### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | Applies the redaction to a given format instance. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### Properties
| Property | Description |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | The count of pages to remove. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | The start position index (0-based). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | The seek reference position, either the beginning or the end of a document. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | The description of the redaction, containing its name and parameters. (inherited from [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Remove 1 page counting from the end of the document
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # Apply the redaction
        result = redactor.apply(rem_opt)

        # Save the redacted document
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
Task guides that use `RemovePageRedaction`:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
