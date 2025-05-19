---
title: RemovePageRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 210
---

## RemovePageRedaction class

Represents a redaction that removes a page (slide, worksheet, etc.) from a document.



**Inheritance:** [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction) → 
[`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)



The RemovePageRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#groupdocs.redaction.redactions.PageSeekOrigin-int-int) | Initializes a new instance of RemovePageRedaction class. |


### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/description) | Returns a string, describing the redaction and its parameters. |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin) | Gets seek reference position, the beginning or the end of a document. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index) | Gets start position index (0-based). |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count) | Gets the count of pages to remove. |


### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#groupdocs.redaction.integration.DocumentFormatInstance) | Applies the redaction to a given format instance. |



### Remarks 


**Learn more** |
|
 |
 |

### Example 


The following example demonstrates how to remove the last page of the document.

### See Also
* module [`groupdocs.redaction.redactions`](..)
* class [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction)
