---
title: MetadataItem
second_title: GroupDocs.Redaction for .NET API Reference
description: Represents an item of metadata common for all supported formats and used in metadata redactions.
type: docs
weight: 210
url: /net/groupdocs.redaction.integration/metadataitem/
---
## MetadataItem class

Represents an item of metadata, common for all supported formats and used in metadata redactions.

```csharp
public class MetadataItem : ISerializable
```

## Constructors

| Name | Description |
| --- | --- |
| [MetadataItem](metadataitem)() | Initializes a new instance. |

## Properties

| Name | Description |
| --- | --- |
| [ActualValue](../../groupdocs.redaction.integration/metadataitem/actualvalue) { get; } | Gets the string representation of the metadata item value. |
| [Category](../../groupdocs.redaction.integration/metadataitem/category) { get; set; } | Gets or sets a category of the metadata item, for example resource ID for an embedded resource metadata item. |
| virtual [DictionaryKey](../../groupdocs.redaction.integration/metadataitem/dictionarykey) { get; } | Gets a dictionary key for [`MetadataCollection`](../metadatacollection), using its OriginalName and other data. |
| [Filter](../../groupdocs.redaction.integration/metadataitem/filter) { get; set; } | Gets or sets a value of [`MetadataFilters`](../../groupdocs.redaction.redactions/metadatafilters), assigned to this metadata item which is used in item filtration. |
| [IsCustom](../../groupdocs.redaction.integration/metadataitem/iscustom) { get; set; } | Gets or sets a value indicating whether this item is custom (added by the authors of the document). |
| [OriginalName](../../groupdocs.redaction.integration/metadataitem/originalname) { get; set; } | Gets or sets an original name of the metadata item, as it appears in the document. |
| [Values](../../groupdocs.redaction.integration/metadataitem/values) { get; set; } | Gets or sets the metadata item value. |

## Methods

| Name | Description |
| --- | --- |
| virtual [CreateClone](../../groupdocs.redaction.integration/metadataitem/createclone)() | Creates a deep clone of current instance. |
| virtual [GetObjectData](../../groupdocs.redaction.integration/metadataitem/getobjectdata)(SerializationInfo, StreamingContext) | Returns information about serializable properties. |

### See Also

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.redaction.dll -->