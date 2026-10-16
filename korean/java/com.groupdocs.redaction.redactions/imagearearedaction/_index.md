---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "이미지 문서의 지정된 영역에 색상 사각형을 배치하는 Redaction을 나타냅니다."
type: docs
weight: 18
url: /ko/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

이미지 문서의 지정된 영역에 색상 사각형을 배치하는 Redaction을 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | 특정 영역 크기를 가리기 위해 ImageAreaRedaction 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getOptions()](#getOptions--) | 가져옵니다 |
RegionReplacementOptions
색상 및 영역 매개변수가 포함된 옵션.
|
|  | [getTopLeft()](#getTopLeft--) | 제거할 영역의 좌상단 위치를 가져옵니다. |
|
|  | [getDescription()](#getDescription--) | 레드액션 및 해당 매개변수를 설명하는 문자열을 반환합니다. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 주어진 형식 인스턴스에 레드액션을 적용합니다. |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


특정 영역 크기를 가리기 위해 ImageAreaRedaction 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | topLeft | java.awt.Point | 좌상단 영역 좌표 |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | 영역 크기 및 색상 |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


가져옵니다
RegionReplacementOptions
색상 및 영역 매개변수가 포함된 옵션.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


제거할 영역의 좌상단 위치를 가져옵니다.


**Returns:**
java.awt.Point - 제거할 영역의 좌상단 위치

### getDescription() {#getDescription--}
```
public String getDescription()
```


레드액션 및 해당 매개변수를 설명하는 문자열을 반환합니다.


**Returns:**
java.lang.String - 레드액션 이름 및 매개변수를 포함하는 텍스트.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


주어진 형식 인스턴스에 레드액션을 적용합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | 레드액션을 적용할 문서 인스턴스 |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

