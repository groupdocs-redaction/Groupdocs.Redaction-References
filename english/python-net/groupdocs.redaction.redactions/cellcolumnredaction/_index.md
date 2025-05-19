---
title: CellColumnRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/cellcolumnredaction/
is_root: false
weight: 20
---

## CellColumnRedaction class

Represents a text redaction that replaces text in a spreadsheet documents (CSV, Excel, etc.).



**Inheritance:** [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction) → 
[`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction) → 
[`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)



The CellColumnRedaction type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/description) | Returns a string, describing the redaction and its parameters. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/action_options) | Gets the [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions) instance, specifying type of text replacement. |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/ocr_connector) | Gets or sets the [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector) implementation, required to extract text from graphic content. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/filter) | Gets the column and worksheet filter. |


### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to/#groupdocs.redaction.integration.DocumentFormatInstance) | Applies the redaction to a given format instance. |



### Remarks 


**Learn more** |
|
 |
 |

### Example 


The following example demonstrates removing user emails from a second column on "Customers" worksheet of a spreadsheet document.

### See Also
* module [`groupdocs.redaction.redactions`](..)
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction)
* class [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector)
* class [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions)
* class [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction)
