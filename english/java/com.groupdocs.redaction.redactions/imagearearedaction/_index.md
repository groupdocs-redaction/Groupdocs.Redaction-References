---
title: ImageAreaRedaction
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a redaction that places colored rectangle in given area of an image document.
type: docs
weight: 16
url: /java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

Represents a redaction that places colored rectangle in given area of an image document.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about image redactions: [Image redactions][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Image redactions]: https://docs.groupdocs.com/redaction/java/image-redactions/
## Constructors

| Constructor | Description |
| --- | --- |
| [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Initializes a new instance of ImageAreaRedaction class for redacting specific area size. |
## Methods

| Method | Description |
| --- | --- |
| [getOptions()](#getOptions--) | Gets the  RegionReplacementOptions  options with color and area parameters. |
| [getTopLeft()](#getTopLeft--) | Gets the top-left position of the area to remove |
| [getDescription()](#getDescription--) | Returns a string, describing the redaction and its parameters. |
| [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applies the redaction to a given format instance. |
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


Initializes a new instance of ImageAreaRedaction class for redacting specific area size.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topLeft | java.awt.Point | Top-left area coordinates |
| options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Area size and color |

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


Gets the  RegionReplacementOptions  options with color and area parameters.

**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.
### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


Gets the top-left position of the area to remove

**Returns:**
java.awt.Point - The top-left position of the area to remove
### getDescription() {#getDescription--}
```
public String getDescription()
```


Returns a string, describing the redaction and its parameters.

**Returns:**
java.lang.String - Text, containing redaction name and parameters.
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
