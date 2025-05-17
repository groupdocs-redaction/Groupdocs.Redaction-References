---
title: AnnotationRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---

## AnnotationRedaction class

Represents a redaction that replaces annotation text (comments, etc.) matching a given regular expression.



**Inheritance:** [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction) → 
[`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)



The AnnotationRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#str-str) | Initializes a new instance of AnnotationRedaction class. |


### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description) | Returns a string, describing the redaction and its parameters. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement) | Gets a textual replacement for matched text. |


### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#groupdocs.redaction.integration.DocumentFormatInstance) | Applies the redaction to a given format instance. |



### Remarks 


**Learn more** |
|
 |
 |

### Example 


The following example demonstrates how to replace the name "John" with "[redacted]" in all annotations.

### See Also
* module [`groupdocs.redaction.redactions`](..)
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction)
* class [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)
