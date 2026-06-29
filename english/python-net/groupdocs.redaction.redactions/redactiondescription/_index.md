---
title: RedactionDescription class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a single change action info that performed during redaction process."
type: docs
url: /python-net/groupdocs.redaction.redactions/redactiondescription/
is_root: false
weight: 200
---


## RedactionDescription class

Represents a single change action info that performed during redaction process.

Learn more

- More details about [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) class and [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: Use redaction callback https://docs.groupdocs.com/redaction/net/use-redaction-callback/

The RedactionDescription type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-original_text) | Initializes a new instance of RedactionDescription class without replacement information. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-original_text-replacement) | Initializes a new instance of RedactionDescription class with replacement information. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-image_area_replacement-image_details) | Initializes a new RedactionDescription with image area replacement information. |

### Properties
| Property | Description |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/action_type/) | The redaction operation: replacement, cleanup or deletion. |
| [details](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/details/) | The optional details information for the item being redacted. |
| [image_area_replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/image_area_replacement/) | The replacement information for image area redactions, or None for textual redactions. |
| [original_text](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/original_text/) | The matched text, if any expression is provided. |
| [redaction_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/redaction_type/) | The type of document's data – text, metadata, or annotations. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/replacement/) | The replacement information, may be None. |

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
