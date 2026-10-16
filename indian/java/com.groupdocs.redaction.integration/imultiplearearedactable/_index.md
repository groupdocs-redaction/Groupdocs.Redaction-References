---
title: "IMultipleAreaRedactable"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "एक ही रंग से कई इमेज क्षेत्रों को एक साथ रेडैक्ट करने के लिए आवश्यक विधियों को परिभाषित करता है।"
type: docs
weight: 22
url: /hi/java/com.groupdocs.redaction.integration/imultiplearearedactable/
---```
public interface IMultipleAreaRedactable
```

Defines methods that are required to redact multiple image areas at once with the same color.

## Methods

| Method | Description |
| --- | --- |
| [getRawStream()](#getRawStream--) | Retrieves a stream with actual image content.
 |
| [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Redacts multiple image areas at once with the same color.
 |
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
| rectangles | java.awt.Rectangle[] | An array of rectangle areas
 |
| boxColor | java.awt.Color | Color to fill the areas
 |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

