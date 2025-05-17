---
title: ExactPhraseRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---

## ExactPhraseRedaction class

Represents a text redaction that replaces exact phrase in the document's text, case insensitive by default.



**Inheritance:** [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction) → 
[`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction) → 
[`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)



The ExactPhraseRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#str-groupdocs.redaction.redactions.ReplacementOptions) | Initializes a new instance of ExactPhraseRedaction class in case insensitive mode. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#str-bool-groupdocs.redaction.redactions.ReplacementOptions) | Initializes a new instance of ExactPhraseRedaction class. |


### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description) | Returns a string, describing the redaction and its parameters. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/action_options) | Gets the [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions) instance, specifying type of text replacement. |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/ocr_connector) | Gets or sets the [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector) implementation, required to extract text from graphic content. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase) | Gets the string to search and replace. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive) | Gets a value indicating whether the search is case-sensitive or not. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left) | Gets or sets a value indicating if this text is right-to-Left or not, false by default. |


### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#groupdocs.redaction.integration.DocumentFormatInstance) | Applies the redaction to a given format instance. |



### Remarks 


**Learn more** |
|
 |
 |

### Example 


The following example demonstrates performing case-sensitive phrase search and replacement.

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

### See Also
* module [`groupdocs.redaction.redactions`](..)
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction)
* class [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector)
* class [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions)
* class [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction)
