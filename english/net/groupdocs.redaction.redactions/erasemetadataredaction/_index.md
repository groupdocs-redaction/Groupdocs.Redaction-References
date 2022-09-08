---
title: EraseMetadataRedaction
second_title: GroupDocs.Redaction for .NET API Reference
description: Represents a metadata redaction that erases all metadata or metadata matching specific MetadataFilters from the document.
type: docs
weight: 470
url: /net/groupdocs.redaction.redactions/erasemetadataredaction/
---
## EraseMetadataRedaction class

Represents a metadata redaction that erases all metadata or metadata matching specific MetadataFilters from the document.

```csharp
public class EraseMetadataRedaction : MetadataRedaction
```

## Constructors

| Name | Description |
| --- | --- |
| [EraseMetadataRedaction](erasemetadataredaction#constructor)() | Initializes a new instance of EraseMetadataRedaction class, erasing all metadata. |
| [EraseMetadataRedaction](erasemetadataredaction#constructor_1)(MetadataFilters) | Initializes a new instance of EraseMetadataRedaction class, erasing metadata, matching specific combination of [`MetadataFilters`](../metadatafilters). |

## Properties

| Name | Description |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/erasemetadataredaction/description) { get; } | Returns a string, describing the redaction and its parameters. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Gets or sets the filter, which is used to select all or specific metadata, for example Author or Company. |

## Methods

| Name | Description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Applies the redaction to a given format instance. |

### Remarks

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Examples

The following example demonstrates how to erase (set equal to empty values) all or specific metadata.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   // Erase Author, Manager and Company
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.Author | MetadataFilters.Manager | MetadataFilters.Company));
   // Erase all metadata
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.All));
   redactor.Save();
}
```

### See Also

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.redaction.dll -->