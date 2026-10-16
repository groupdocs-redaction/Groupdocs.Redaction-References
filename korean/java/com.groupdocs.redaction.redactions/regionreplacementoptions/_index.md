---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "이미지 영역 교체를 위한 색상 및 영역 매개변수를 나타냅니다."
type: docs
weight: 29
url: /ko/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

이미지 영역 교체를 위한 색상 및 영역 매개변수를 나타냅니다. 참조
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | RegionReplacementOptions 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | 주어진 텍스트와 크기가 일치하는 RegionReplacementOptions 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | 삭제된 영역을 채우는 색상을 가져옵니다. |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | 삭제된 영역을 채우는 색상을 설정합니다. |
|
|  | [getSize()](#getSize--) | 사각형의 너비와 높이를 가져옵니다. |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | 사각형의 너비와 높이를 설정합니다. |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


RegionReplacementOptions 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | fillColor | java.awt.Color | 영역을 채우는 색상 |
|
|  | 크기 | java.awt.Dimension | 채워진 영역 크기 |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


주어진 텍스트와 크기가 일치하는 RegionReplacementOptions 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | fillColor | java.awt.Color | 영역을 채우는 색상 |
|
|  | font | java.awt.Font | 예상 텍스트 폰트 |
|
|  | expectedText | java.lang.String | 예상 텍스트 |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


삭제된 영역을 채우는 색상을 가져옵니다.


**Returns:**
java.awt.Color - 가려진 영역을 채우는 색상.

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


삭제된 영역을 채우는 색상을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.awt.Color | 가려진 영역을 채우는 색상. |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


사각형의 너비와 높이를 가져옵니다.


**Returns:**
java.awt.Dimension - 사각형의 너비와 높이.

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


사각형의 너비와 높이를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.awt.Dimension | 사각형의 너비와 높이. |
|

