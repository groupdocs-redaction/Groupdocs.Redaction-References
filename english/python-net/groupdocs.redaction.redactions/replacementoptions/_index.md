---
title: ReplacementOptions class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 220
---

## ReplacementOptions class

Represents options for matched text replacement.



The ReplacementOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#str) | Initializes a new instance of ReplacementOptions class with replacement text as an option. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#aspose.pydrawing.Color) | Initializes a new instance of ReplacementOptions class with colored rectangle as an option. |


### Properties
| Property | Description |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type) | Gets the replacement action: draw box or replace text. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement) | Gets or sets the textual replacement value. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color) | Gets or sets the color for a [`ReplacementType.DRAW_BOX`](/redaction/python-net/groupdocs.redaction.redactions/replacementtype#DRAW_BOX) option (ignored otherwise). |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters) | Gets or sets an array of filters to apply with this redaction. |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction) | Gets or sets a custom redaction [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler) handler that allows users to define their own redaction logic. |



### Remarks 


**Learn more** |
|
 |
 |

### See Also
* module [`groupdocs.redaction.redactions`](..)
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler)
