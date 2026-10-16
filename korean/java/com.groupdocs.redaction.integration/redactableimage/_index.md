---
title: "RedactableImage"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "모든 래스터 이미지 삭제 작업에 대한 파사드를 제공합니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

모든 래스터 이미지 삭제 작업에 대한 파사드를 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | 객체를 사용하여 구현하는 새 인스턴스를 생성합니다. |
IImageFormatInstance
인터페이스.
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | 객체를 사용하여 구현하는 새 인스턴스를 생성합니다. |
IMultipleAreaRedactable
인터페이스.
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | 실제 이미지 콘텐츠가 포함된 스트림을 검색합니다. |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | 동일한 색상으로 여러 이미지 영역을 한 번에 가립니다. |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | 주어진 지점의 영역을 특정 색상과 크기의 사각형으로 교체합니다. |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


객체를 사용하여 구현하는 새 인스턴스를 생성합니다.
IImageFormatInstance
인터페이스.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | IImageFormatInstance 인터페이스를 구현하는 인스턴스 |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


객체를 사용하여 구현하는 새 인스턴스를 생성합니다.
IMultipleAreaRedactable
인터페이스.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | IMultipleAreaRedactable 인터페이스를 구현하는 인스턴스 |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


실제 이미지 콘텐츠가 포함된 스트림을 검색합니다.


**Returns:**
java.io.InputStream - 이미지 데이터를 포함하는 스트림

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


동일한 색상으로 여러 이미지 영역을 한 번에 가립니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 사각형들 | java.awt.Rectangle[] | 사각형 영역의 배열 |
|
|  | boxColor | java.awt.Color | 영역을 채우는 색상 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


주어진 지점의 영역을 특정 색상과 크기의 사각형으로 교체합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | topLeft | java.awt.Point | 채워진 영역의 왼쪽 위 모서리 좌표 |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | 색상 및 크기 설정 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

