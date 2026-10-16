---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "일치된 텍스트 교체 옵션을 나타냅니다."
type: docs
weight: 31
url: /ko/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

일치된 텍스트 교체 옵션을 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | ReplacementOptions 클래스의 새 인스턴스를 초기화하며, 옵션으로 교체 텍스트를 사용합니다. |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | ReplacementOptions 클래스의 새 인스턴스를 초기화하며, 옵션으로 색상 사각형을 사용합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getActionType()](#getActionType--) | 교체 작업을 가져옵니다: 상자 그리기 또는 텍스트 교체. |
|
|  | [getReplacement()](#getReplacement--) | 텍스트 교체 값을 가져옵니다. |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | 텍스트 교체 값을 설정합니다. |
|
|  | [getBoxColor()](#getBoxColor--) | a에 대한 색상을 가져옵니다. |
ReplacementType.DrawBox
옵션 (다른 경우 무시됨).
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | 색상을 설정합니다 |
ReplacementType.DrawBox
옵션 (다른 경우 무시됨).
|
|  | [getFilters()](#getFilters--) | 이 리다크션에 적용할 필터 배열을 가져옵니다. |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | 이 리다크션에 적용할 필터 배열을 설정합니다. |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | 사용자 지정 리다크션 핸들러를 가져옵니다. |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | 사용자 지정 리다크션 핸들러를 설정합니다. |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


ReplacementOptions 클래스의 새 인스턴스를 초기화하며, 옵션으로 교체 텍스트를 사용합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 대체 | java.lang.String | 텍스트 대체 |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


ReplacementOptions 클래스의 새 인스턴스를 초기화하며, 옵션으로 색상 사각형을 사용합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 색상 | java.awt.Color | 사각형 색상 |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


교체 작업을 가져옵니다: 상자 그리기 또는 텍스트 교체.


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


텍스트 교체 값을 가져옵니다.


**Returns:**
java.lang.String - 텍스트 대체 값.

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


텍스트 교체 값을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 텍스트 대체 값. |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


a에 대한 색상을 가져옵니다.
ReplacementType.DrawBox
옵션 (다른 경우 무시됨).


**Returns:**
java.awt.Color - ReplacementType.DrawBox 옵션에 대한 색상 (다른 경우 무시됨).

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


색상을 설정합니다
ReplacementType.DrawBox
옵션 (다른 경우 무시됨).


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.awt.Color | ReplacementType.DrawBox 옵션에 대한 색상 (다른 경우 무시됨). |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


이 리다크션에 적용할 필터 배열을 가져옵니다.


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - 이 리다크션에 적용할 필터 배열.

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


이 리다크션에 적용할 필터 배열을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | 이 리다크션에 적용할 필터 배열. |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


사용자 지정 리다크션 핸들러를 가져옵니다. PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction)에서만 지원됩니다.


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


사용자 지정 리다크션 핸들러를 설정합니다. PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction)에서만 지원됩니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | 다음의 인스턴스인 [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler). |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
