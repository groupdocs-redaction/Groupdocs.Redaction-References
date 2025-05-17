---
title: MetadataItem class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.integration/metadataitem/
is_root: false
weight: 120
---

## MetadataItem class

Represents an item of metadata, common for all supported formats and used in metadata redactions.



The MetadataItem type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.integration/metadataitem/__init__/#) | Initializes a new instance. |


### Properties
| Property | Description |
| :- | :- |
| [original_name](/redaction/python-net/groupdocs.redaction.integration/metadataitem/original_name) | Gets or sets an original name of the metadata item, as it appears in the document. |
| [category](/redaction/python-net/groupdocs.redaction.integration/metadataitem/category) | Gets or sets a category of the metadata item, for example resource ID for an embedded resource metadata item. |
| [filter](/redaction/python-net/groupdocs.redaction.integration/metadataitem/filter) | Gets or sets a value of [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters), assigned to this metadata item which is used in item filtration. |
| [values](/redaction/python-net/groupdocs.redaction.integration/metadataitem/values) | Gets or sets the metadata item value. |
| [is_custom](/redaction/python-net/groupdocs.redaction.integration/metadataitem/is_custom) | Gets or sets a value indicating whether this item is custom (added by the authors of the document). |
| [dictionary_key](/redaction/python-net/groupdocs.redaction.integration/metadataitem/dictionary_key) | Gets a dictionary key for [`MetadataCollection`](/redaction/python-net/groupdocs.redaction.integration/metadatacollection), using its OriginalName and other data. |
| [actual_value](/redaction/python-net/groupdocs.redaction.integration/metadataitem/actual_value) | Gets the string representation of the metadata item value. |


### Methods
| Method | Description |
| :- | :- |
| [create_clone](/redaction/python-net/groupdocs.redaction.integration/metadataitem/create_clone/#) | Creates a deep clone of current instance. |



### See Also
* module [`groupdocs.redaction.integration`](..)
* class [`MetadataCollection`](/redaction/python-net/groupdocs.redaction.integration/metadatacollection)
* class [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters)
