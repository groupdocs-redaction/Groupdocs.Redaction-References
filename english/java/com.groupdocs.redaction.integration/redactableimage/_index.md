---
title: RedactableImage
second_title: GroupDocs.Redaction for Java API Reference
description: Provides facade to all raster image redaction operations.
type: docs
weight: 14
url: /java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

Provides facade to all raster image redaction operations.
## Constructors

| Constructor | Description |
| --- | --- |
| [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | Creates a new instace using an object, implementing  IImageFormatInstance  interface. |
| [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | Creates a new instace using an object, implementing  IMultipleAreaRedactable  interface. |
## Methods

| Method | Description |
| --- | --- |
| [getRawStream()](#getRawStream--) | Retrieves a stream with actual image content. |
| [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Redacts multiple image areas at once with the same color. |
| [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Replaces the area at given point with a rectangle of specific color and size. |
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


Creates a new instace using an object, implementing  IImageFormatInstance  interface.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | An instance, implementing IImageFormatInstance interface |

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


Creates a new instace using an object, implementing  IMultipleAreaRedactable  interface.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | An instance, implementing IMultipleAreaRedactable interface |

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


Retrieves a stream with actual image content.

**Returns:**
java.io.InputStream - Stream, containing image data
### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


Redacts multiple image areas at once with the same color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangles | java.awt.Rectangle[] | An array of rectangle areas |
| boxColor | java.awt.Color | Color to fill the areas |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result
### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Replaces the area at given point with a rectangle of specific color and size.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topLeft | java.awt.Point | Top-left corner coordinates of filled area |
| options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Color and size settings |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result
