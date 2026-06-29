---
title: AnnotationRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a redaction that replaces annotation text (comments, etc.) matching a given regular expression."
type: docs
url: /python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

Represents a redaction that replaces annotation text (comments, etc.) matching a given regular expression.

Learn more

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

The AnnotationRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | Initializes a new AnnotationRedaction with a regex pattern and replacement text. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | Initializes a new instance of [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/). |

### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | Applies the redaction to a given format instance. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | The description of the redaction, describing the redaction and its parameters. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | The regular expression to match. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | The textual replacement for matched text. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
Task guides that use `AnnotationRedaction`:

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
