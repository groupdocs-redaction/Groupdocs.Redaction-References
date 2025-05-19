---
title: EraseMetadataRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---

## EraseMetadataRedaction class

Represents a metadata redaction that erases all metadata or metadata matching specific MetadataFilters from the document.



**Inheritance:** [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction) → 
[`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction) → 
[`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)



The EraseMetadataRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#) | Initializes a new instance of EraseMetadataRedaction class, erasing all metadata. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#groupdocs.redaction.redactions.MetadataFilters) | Initializes a new instance of EraseMetadataRedaction class, erasing metadata, matching specific combination of [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters). |


### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description) | Returns a string, describing the redaction and its parameters. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/filter) | Gets or sets the filter, which is used to select all or specific metadata, for example Author or Company. |


### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/apply_to/#groupdocs.redaction.integration.DocumentFormatInstance) | Applies the redaction to a given format instance. |



### Remarks 


**Learn more** |
|
 |
 |

### Example 


The following example demonstrates how to erase (set equal to empty values) all or specific metadata.

### See Also
* module [`groupdocs.redaction.redactions`](..)
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction)
* class [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters)
* class [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction)
* class [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)
