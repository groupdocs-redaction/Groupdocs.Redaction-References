---
title: "IMultipleAreaRedactable"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "동일한 색상으로 여러 이미지 영역을 한 번에 삭제하기 위해 필요한 메서드를 정의합니다."
type: docs
weight: 22
url: /ko/java/com.groupdocs.redaction.integration/imultiplearearedactable/
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

