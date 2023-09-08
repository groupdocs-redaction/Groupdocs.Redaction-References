---
title: IImageFormatInstance
second_title: GroupDocs.Redaction for Java API Reference
description: Defines methods that are required for raster image format redactions.
type: docs
weight: 21
url: /java/com.groupdocs.redaction.integration/iimageformatinstance/
---```
public interface IImageFormatInstance
```

Defines methods that are required for raster image format redactions.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about image redactions: [Image redactions][]
 *  More details about implementing custom formats: [Create custom format handler][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Image redactions]: https://docs.groupdocs.com/redaction/java/image-redactions/
[Create custom format handler]: https://docs.groupdocs.com/redaction/java/create-custom-format-handler/
## Methods

| Method | Description |
| --- | --- |
| [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Replaces the area at given point with a rectangle of specific color and size. |
### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public abstract RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Replaces the area at given point with a rectangle of specific color and size.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topLeft | java.awt.Point | Top-left corner coordinates of filled area |
| options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Color and size settings |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result
