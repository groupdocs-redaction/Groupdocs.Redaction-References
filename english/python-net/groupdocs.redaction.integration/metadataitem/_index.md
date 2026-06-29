---
title: MetadataItem class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents an item of metadata, common for all supported formats and used in metadata redactions."
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
| [__init__](/redaction/python-net/groupdocs.redaction.integration/metadataitem/__init__/) | Initializes a new instance. |

### Methods
| Method | Description |
| :- | :- |
| [create_clone](/redaction/python-net/groupdocs.redaction.integration/metadataitem/create_clone/) | Creates a deep clone of the current instance. |
| [get_object_data](/redaction/python-net/groupdocs.redaction.integration/metadataitem/get_object_data/#info-context) | Returns information about serializable properties. |
| [get_object_data_serialization_info](/redaction/python-net/groupdocs.redaction.integration/metadataitem/get_object_data_serialization_info/) |  |

### Properties
| Property | Description |
| :- | :- |
| [actual_value](/redaction/python-net/groupdocs.redaction.integration/metadataitem/actual_value/) | The string representation of the metadata item value. |
| [category](/redaction/python-net/groupdocs.redaction.integration/metadataitem/category/) | The category of the metadata item, for example resource ID for an embedded resource metadata item. |
| [dictionary_key](/redaction/python-net/groupdocs.redaction.integration/metadataitem/dictionary_key/) | The dictionary key for a [`MetadataCollection`](/redaction/python-net/groupdocs.redaction.integration/metadatacollection/), derived from its OriginalName and other data. |
| [filter](/redaction/python-net/groupdocs.redaction.integration/metadataitem/filter/) | The filter assigned to this metadata item, represented by a `MetadataFilters` value, used for item filtration. |
| [is_custom](/redaction/python-net/groupdocs.redaction.integration/metadataitem/is_custom/) | The item is custom (added by the authors of the document). |
| [original_name](/redaction/python-net/groupdocs.redaction.integration/metadataitem/original_name/) | The original name of the metadata item as it appears in the document. |
| [values](/redaction/python-net/groupdocs.redaction.integration/metadataitem/values/) | The metadata item value. |

### See Also
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
