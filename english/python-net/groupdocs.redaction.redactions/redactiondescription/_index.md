---
title: RedactionDescription class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/redactiondescription/
is_root: false
weight: 170
---

## RedactionDescription class

Represents a single change action info that performed during redaction process.



The RedactionDescription type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#groupdocs.redaction.redactions.RedactionType-groupdocs.redaction.redactions.RedactionActionType-str) | Initializes a new instance of RedactionDescription class without replacement information. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#groupdocs.redaction.redactions.RedactionType-groupdocs.redaction.redactions.RedactionActionType-str-groupdocs.redaction.redactions.TextReplacement) | Initializes a new instance of RedactionDescription class with replacement information. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#groupdocs.redaction.redactions.RedactionType-groupdocs.redaction.redactions.RedactionActionType-groupdocs.redaction.redactions.RegionReplacementOptions-str) | Initializes a new instance of RedactionDescription class with image area replacement information. |


### Properties
| Property | Description |
| :- | :- |
| [redaction_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/redaction_type) | Gets the type of document's data - text, metadata or annotations. |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/action_type) | Gets the redaction operation: replacement, cleanup or deletion. |
| [original_text](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/original_text) | Gets the matched text, if any expression is provided. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/replacement) | Gets the replacement information, can be null. |
| [image_area_replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/image_area_replacement) | Gets the replacement information for image area redactions, returns null for textual redactions. |
| [details](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/details) | Gets or sets an optional details information for the item being redacted. |



### Remarks 


**Learn more** |
|
 |

### See Also
* module [`groupdocs.redaction.redactions`](..)
