---
title: PageAreaRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 150
---

## PageAreaRedaction class

Represents a complex textual redaction that affects text, images and annotations in an area of the page.



**Inheritance:** [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction) → 
[`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction) → 
[`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction) → 
[`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)



The PageAreaRedaction type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/description) | Returns a string, describing the redaction and its parameters. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/action_options) | Gets the [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions) instance, specifying type of text replacement. |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/ocr_connector) | Gets or sets the [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector) implementation, required to extract text from graphic content. |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options) | Gets the [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions) options with color and area parameters. |


### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#groupdocs.redaction.integration.DocumentFormatInstance) | Applies the redaction to a given format instance. |



### Remarks 


**Learn more** |
|
 |
 |

### See Also
* module [`groupdocs.redaction.redactions`](..)
* class [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector)
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction)
* class [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction)
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions)
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions)
* class [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction)
