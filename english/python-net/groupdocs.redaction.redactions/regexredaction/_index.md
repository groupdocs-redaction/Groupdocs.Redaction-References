---
title: RegexRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 190
---

## RegexRedaction class

Represents a text redaction that searches and replaces text in the document by matching provided regular expression.



**Inheritance:** [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction) → 
[`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction) → 
[`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)



The RegexRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#str-groupdocs.redaction.redactions.ReplacementOptions) | Initializes a new instance of RegexRedaction class. |


### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description) | Returns a string, describing the redaction and its parameters. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/action_options) | Gets the [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions) instance, specifying type of text replacement. |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/ocr_connector) | Gets or sets the [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector) implementation, required to extract text from graphic content. |


### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#groupdocs.redaction.integration.DocumentFormatInstance) | Applies the redaction to a given format instance. |



### Remarks 


**Learn more** |
|
 |
 |

### Example 


The following example demonstrates replacing text using the regular expression.

### See Also
* module [`groupdocs.redaction.redactions`](..)
* class [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector)
* class [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction)
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions)
* class [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction)
