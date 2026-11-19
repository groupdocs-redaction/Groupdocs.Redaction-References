---
title: DeleteAnnotationRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a text redaction that deletes annotations if text matches the given regular expression (optionally deletes all annotations)."
type: docs
url: /python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

Represents a text redaction that deletes annotations if text matches the given regular expression (optionally deletes all annotations).

Learn more:
- More details about applying redactions: https://docs.groupdocs.com/redaction/python-net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/python-net/annotation-redactions/

The DeleteAnnotationRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | Initializes a new DeleteAnnotationRedaction instance that deletes all annotations (matches everything). |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching the given regular expression. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching given expression. |

### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | Applies the redaction to a given format instance. |

### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | The description of the redaction, containing its name and parameters. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | The regular expression to match. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # Delete annotations containing the word "internal" (case‑insensitive)
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
Task guides that use `DeleteAnnotationRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Use advanced logging](/redaction/python-net/guides/use-advanced-logging/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
