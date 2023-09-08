---
title: IMetadataAccess
second_title: GroupDocs.Redaction for Java API Reference
description: Defines methods that are required for access to metadata of a document if format supports it.
type: docs
weight: 22
url: /java/com.groupdocs.redaction.integration/imetadataaccess/
---```
public interface IMetadataAccess
```

Defines methods that are required for access to metadata of a document, if format supports it.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about document metadata redactions: [Metadata redactions][]
 *  More details about implementing custom formats: [Create custom format handler][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Metadata redactions]: https://docs.groupdocs.com/redaction/java/metadata-redactions/
[Create custom format handler]: https://docs.groupdocs.com/redaction/java/create-custom-format-handler/
## Methods

| Method | Description |
| --- | --- |
| [getMetadata()](#getMetadata--) | Retrieves a dictionary with document's metadata. |
| [changeMetadata(MetadataItem metadataItem)](#changeMetadata-com.groupdocs.redaction.integration.MetadataItem-) | Changes the specified item of metadata from or adds a new one, if not present. |
### getMetadata() {#getMetadata--}
```
public abstract MetadataCollection getMetadata()
```


Retrieves a dictionary with document's metadata.

**Returns:**
[MetadataCollection](../../com.groupdocs.redaction.integration/metadatacollection) - Plain dictionary with metadata
### changeMetadata(MetadataItem metadataItem) {#changeMetadata-com.groupdocs.redaction.integration.MetadataItem-}
```
public abstract RedactionResult changeMetadata(MetadataItem metadataItem)
```


Changes the specified item of metadata from or adds a new one, if not present.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| metadataItem | [MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) | Metadata item with a new value assigned to it |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Metadata redaction result
