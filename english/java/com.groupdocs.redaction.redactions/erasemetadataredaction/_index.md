---
title: EraseMetadataRedaction
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a metadata redaction that erases all metadata or metadata matching specific MetadataFilters from the document.
type: docs
weight: 14
url: /java/com.groupdocs.redaction.redactions/erasemetadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.MetadataRedaction](../../com.groupdocs.redaction.redactions/metadataredaction)
```
public class EraseMetadataRedaction extends MetadataRedaction
```

Represents a metadata redaction that erases all metadata or metadata matching specific MetadataFilters from the document.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about document metadata redactions: [Metadata redactions][]

The following example demonstrates how to erase (set equal to empty values) all or specific metadata.

```

  try (Redactor redactor = new Redactor("C:\\sample.docx"))
 {
    // Erase Author, Manager and Company
    redactor.apply(new EraseMetadataRedaction(MetadataFilters.Author | MetadataFilters.Manager | MetadataFilters.Company));
    // Erase all metadata
    redactor.apply(new EraseMetadataRedaction(MetadataFilters.All));
    redactor.save();
 }
 
```


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Metadata redactions]: https://docs.groupdocs.com/redaction/java/metadata-redactions/
## Constructors

| Constructor | Description |
| --- | --- |
| [EraseMetadataRedaction()](#EraseMetadataRedaction--) | Initializes a new instance of EraseMetadataRedaction class, erasing all metadata. |
| [EraseMetadataRedaction(int filter)](#EraseMetadataRedaction-int-) | Initializes a new instance of EraseMetadataRedaction class, erasing metadata, matching specific combination of  MetadataFilters . |
## Methods

| Method | Description |
| --- | --- |
| [getDescription()](#getDescription--) | Returns a string, describing the redaction and its parameters. |
### EraseMetadataRedaction() {#EraseMetadataRedaction--}
```
public EraseMetadataRedaction()
```


Initializes a new instance of EraseMetadataRedaction class, erasing all metadata.

### EraseMetadataRedaction(int filter) {#EraseMetadataRedaction-int-}
```
public EraseMetadataRedaction(int filter)
```


Initializes a new instance of EraseMetadataRedaction class, erasing metadata, matching specific combination of  MetadataFilters .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filter | int | Filter for metadata to erase |

### getDescription() {#getDescription--}
```
public String getDescription()
```


Returns a string, describing the redaction and its parameters.

**Returns:**
java.lang.String - Text, containing redaction name and parameters.
