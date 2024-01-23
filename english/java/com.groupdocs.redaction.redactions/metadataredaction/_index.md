---
title: MetadataRedaction
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a base abstract class for document metadata redactions.
type: docs
weight: 18
url: /java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

Represents a base abstract class for document metadata redactions.

--------------------

**Learn more**

 *  More details about document metadata redactions: [Metadata redactions][]


[Metadata redactions]: https://docs.groupdocs.com/redaction/java/metadata-redactions/
## Methods

| Method | Description |
| --- | --- |
| [getFilter()](#getFilter--) | Gets the filter, which is used to select all or specific metadata, for example Author or Company. |
| [setFilter(int value)](#setFilter-int-) | Sets the filter, which is used to select all or specific metadata, for example Author or Company. |
| [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applies the redaction to a given format instance. |
### getFilter() {#getFilter--}
```
public final int getFilter()
```


Gets the filter, which is used to select all or specific metadata, for example Author or Company.

**Returns:**
int - The filter, which is used to select all or specific metadata, for example Author or Company.
### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Sets the filter, which is used to select all or specific metadata, for example Author or Company.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The filter, which is used to select all or specific metadata, for example Author or Company. |

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applies the redaction to a given format instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | An instance of a document to apply redaction |

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any
