---
title: RedactionDescription class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
weight: 170
url: /groupdocs.redaction.redactions/redactiondescription/
is_root: false
---

## RedactionDescription class

Represents a single change action info that performed during redaction process.



The RedactionDescription type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self, redaction_type, action_type, original_text)`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#groupdocs.redaction.redactions.redactiontype-groupdocs.redaction.redactions.redactionactiontype-str) | Initializes a new instance of RedactionDescription class without replacement information. |
| [`__init__(self, redaction_type, action_type, original_text, replacement)`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#groupdocs.redaction.redactions.redactiontype-groupdocs.redaction.redactions.redactionactiontype-str-groupdocs.redaction.redactions.textreplacement) | Initializes a new instance of RedactionDescription class with replacement information. |
| [`__init__(self, redaction_type, action_type, image_area_replacement, image_details)`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#groupdocs.redaction.redactions.redactiontype-groupdocs.redaction.redactions.redactionactiontype-groupdocs.redaction.redactions.regionreplacementoptions-str) | Initializes a new instance of RedactionDescription class with image area replacement information. |


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
