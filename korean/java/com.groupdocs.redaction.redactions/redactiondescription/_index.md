---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "삭제 과정 중 수행된 단일 변경 작업 정보를 나타냅니다."
type: docs
weight: 25
url: /ko/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

삭제 과정 중 수행된 단일 변경 작업 정보를 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | 대체 정보 없이 RedactionDescription 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | 대체 정보를 포함하여 RedactionDescription 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | 이미지 영역 대체 정보를 포함하여 RedactionDescription 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | 문서 데이터 유형을 가져옵니다 - 텍스트, 메타데이터 또는 주석. |
|
|  | [getActionType()](#getActionType--) | 마스킹 작업을 가져옵니다: 교체, 정리 또는 삭제. |
|
|  | [getOriginalText()](#getOriginalText--) | 표현식이 제공된 경우 일치하는 텍스트를 가져옵니다. |
|
|  | [getReplacement()](#getReplacement--) | 교체 정보를 가져옵니다. null일 수 있습니다. |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | 이미지 영역 마스킹에 대한 교체 정보를 가져옵니다. 텍스트 마스킹의 경우 null을 반환합니다. |
|
|  | [getDetails()](#getDetails--) | 마스킹되는 항목에 대한 선택적 상세 정보를 가져옵니다. |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | 마스킹되는 항목에 대한 선택적 상세 정보를 설정합니다. |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


대체 정보 없이 RedactionDescription 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | redactionType | int | 마스킹되는 데이터 유형 |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | 이 데이터에 수행될 작업 |
|
|  | originalText | java.lang.String | 일치하는 �스트, 주석 또는 어노테이션 본문 |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


대체 정보를 포함하여 RedactionDescription 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | redactionType | int | 마스킹되는 데이터 유형 |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | 이 데이터에 수행될 작업 |
|
|  | originalText | java.lang.String | 일치하는 �스트, 주석 또는 어노테이션 본문 |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | 교체 텍스트, 일치하는 텍스트 및 원본 문자열 내 위치 |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


이미지 영역 대체 정보를 포함하여 RedactionDescription 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | redactionType | int | 마스킹되는 데이터 유형 |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | 이 데이터에 수행될 작업 |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | 이미지 영역 교체 정보 |
|
|  | imageDetails | java.lang.String | 이미지 텍스트 설명, 기본값은 String.Empty입니다. |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


문서 데이터 유형을 가져옵니다 - 텍스트, 메타데이터 또는 주석.


**Returns:**
int - 문서 데이터 유형 - 텍스트, 메타데이터 또는 어노테이션.

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


마스킹 작업을 가져옵니다: 교체, 정리 또는 삭제.


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


표현식이 제공된 경우 일치하는 텍스트를 가져옵니다.


**Returns:**
java.lang.String - 제공된 표현식이 있는 경우 일치하는 텍스트.

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


교체 정보를 가져옵니다. null일 수 있습니다.


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


이미지 영역 마스킹에 대한 교체 정보를 가져옵니다. 텍스트 마스킹의 경우 null을 반환합니다.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


마스킹되는 항목에 대한 선택적 상세 정보를 가져옵니다.


**Returns:**
java.lang.String - 마스킹되는 항목에 대한 선택적 상세 정보.

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


마스킹되는 항목에 대한 선택적 상세 정보를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 마스킹되는 항목에 대한 선택적 상세 정보. |
|

