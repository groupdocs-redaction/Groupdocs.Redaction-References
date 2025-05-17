---
title: MetadataSearchRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 130
---

## MetadataSearchRedaction class

Represents a metadata redaction that searches and redacts metadata using regular expressions, matching keys and/or values.



**Inheritance:** [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction) → 
[`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction) → 
[`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)



The MetadataSearchRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#str-str) | Initializes a new instance of MetadataSearchRedaction class, using value to match redacted items. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#str-str-str) | Initializes a new instance of MetadataSearchRedaction class, using item name and value to match redacted items. |


### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description) | Returns a string, describing the redaction and its parameters. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/filter) | Gets or sets the filter, which is used to select all or specific metadata, for example Author or Company. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement) | Gets the textual replacement value. |


### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/apply_to/#groupdocs.redaction.integration.DocumentFormatInstance) | Applies the redaction to a given format instance. |



### Remarks 


**Learn more** |
|
 |
 |

### Example 


The following example demonstrates how to search and redact certain text in specific metadata.

### See Also
* module [`groupdocs.redaction.redactions`](..)
* class [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction)
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction)
* class [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)
