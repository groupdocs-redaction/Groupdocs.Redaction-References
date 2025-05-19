---
title: DeleteAnnotationRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---

## DeleteAnnotationRedaction class

Represents a text redaction that deletes annotations if text is matching given regular expression (optionally deletes all annotations).



**Inheritance:** [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction) → 
[`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)



The DeleteAnnotationRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#) | Initializes a new instance of DeleteAnnotationRedaction class, with settings to delete all annotations (matching everything). |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#str) | Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching given expression. |


### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description) | Returns a string, describing the redaction and its parameters. |


### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#groupdocs.redaction.integration.DocumentFormatInstance) | Applies the redaction to a given format instance. |



### Remarks 


**Learn more** |
|
 |
 |

### Example 


The following example demonstrates how to remove all annotations containing words "use", "show" or "describe" from document (and leave others).

### See Also
* module [`groupdocs.redaction.redactions`](..)
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction)
* class [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)
