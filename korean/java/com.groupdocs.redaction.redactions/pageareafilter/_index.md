---
title: "PageAreaFilter"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "문서 페이지 내에서 영역을 설정하여 검열을 적용하는 검열 필터를 나타냅니다."
type: docs
weight: 22
url: /ko/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

문서 페이지 내에서 삭제를 적용할 영역을 설정하는 삭제 필터를 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | 특정 영역을 검열하기 위해 PageAreaFilter 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 페이지에서 사각형(좌상단 위치와 영역 크기)을 가져옵니다. |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | 이 필터 영역이 주어진 사각형과 교차하는지 확인합니다. |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


특정 영역을 검열하기 위해 PageAreaFilter 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | topLeft | java.awt.Point | 좌상단 영역 좌표 |
|
|  | 크기 | java.awt.Dimension | 영역 크기 및 색상 |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


페이지에서 사각형(좌상단 위치와 영역 크기)을 가져옵니다.


**Returns:**
java.awt.Rectangle - 페이지에서 사각형(좌상단 위치와 영역 크기)

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


이 필터 영역이 주어진 사각형과 교차하는지 확인합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 사각형 | java.awt.Rectangle | 확인할 사각형 |
|

**Returns:**
boolean - 이 필터 영역이 교차하면 true

