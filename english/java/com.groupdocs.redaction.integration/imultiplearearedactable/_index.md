---
title: IMultipleAreaRedactable
second_title: GroupDocs.Redaction for Java API Reference
description: Defines methods that are required to redact multiple image areas at once with the same color.
type: docs
weight: 23
url: /java/com.groupdocs.redaction.integration/imultiplearearedactable/
---```
public interface IMultipleAreaRedactable
```

Defines methods that are required to redact multiple image areas at once with the same color.
## Methods

| Method | Description |
| --- | --- |
| [getRawStream()](#getRawStream--) | Retrieves a stream with actual image content. |
| [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Redacts multiple image areas at once with the same color. |
### getRawStream() {#getRawStream--}
```
public abstract InputStream getRawStream()
```


Retrieves a stream with actual image content.

**Returns:**
java.io.InputStream - Stream, containing image data
### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public abstract RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


Redacts multiple image areas at once with the same color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangles | java.awt.Rectangle[] | An array of rectangle areas |
| boxColor | java.awt.Color | Color to fill the areas |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result
