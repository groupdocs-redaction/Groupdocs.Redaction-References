---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "가장 일반적인 문서 메타데이터 유형 목록을 나타냅니다."
type: docs
weight: 19
url: /ko/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

가장 일반적인 문서 메타데이터 유형 목록을 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## 필드

| 필드 | 설명 |
| --- | --- |
|  | [None](#None) | 빈 필터 설정으로, 메타데이터 항목과 일치하지 않습니다. |
|
|  | [Author](#Author) | 문서의 작성자. |
|
|  | [Category](#Category) | 문서의 카테고리. |
|
|  | [Comments](#Comments) | 문서에 대한 주석. |
|
|  | [Company](#Company) | 작성자의 회사. |
|
|  | [ContentStatus](#ContentStatus) | 콘텐츠 상태. |
|
|  | [CreatedTime](#CreatedTime) | 생성 시간. |
|
|  | [HyperlinkBase](#HyperlinkBase) | 하이퍼링크 기본값. |
|
|  | [LastPrinted](#LastPrinted) | 마지막 인쇄 날짜 및 시간. |
|
|  | [LastSavedBy](#LastSavedBy) | 사용자가 마지막으로 저장함. |
|
|  | [LastSavedTime](#LastSavedTime) | 마지막 저장 날짜 및 시간. |
|
|  | [NameOfApplication](#NameOfApplication) | 문서가 생성된 애플리케이션 이름. |
|
|  | [Manager](#Manager) | 작성자 관리자 이름. |
|
|  | [RevisionNumber](#RevisionNumber) | 수정 번호. |
|
|  | [Subject](#Subject) | 문서의 주제. |
|
|  | [Template](#Template) | 문서 템플릿 이름. |
|
|  | [Title](#Title) | 문서 제목. |
|
|  | [TotalEditingTime](#TotalEditingTime) | 총 편집 시간. |
|
|  | [Version](#Version) | 문서 버전. |
|
|  | [Description](#Description) | 문서 설명. |
|
|  | [Keywords](#Keywords) | 문서 키워드. |
|
|  | [ContentType](#ContentType) | 콘텐츠 유형. |
|
|  | [All](#All) | 메타데이터 항목의 모든 유형. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getNames()](#getNames--) | 선언된 모든 필터 유형을 포함하는 집합을 가져옵니다. |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | MetadataFiler의 값을 이름으로 가져옵니다. |
|
|  | [parse(String values)](#parse-java.lang.String-) | 쉼표로 구분된 MetadataFilers 값 문자열을 정수로 구문 분석합니다. |
|
|  | [toString(int value)](#toString-int-) | 정수를 쉼표로 구분된 MetadataFilers 값 문자열로 저장합니다. |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


빈 필터 설정으로, 메타데이터 항목과 일치하지 않습니다.


### Author {#Author}
```
public static final int Author
```


문서의 작성자.


### Category {#Category}
```
public static final int Category
```


문서의 카테고리.


### Comments {#Comments}
```
public static final int Comments
```


문서에 대한 주석.


### Company {#Company}
```
public static final int Company
```


작성자의 회사.


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


콘텐츠 상태.


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


생성 시간.


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


하이퍼링크 기본값.


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


마지막 인쇄 날짜 및 시간.


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


사용자가 마지막으로 저장함.


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


마지막 저장 날짜 및 시간.


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


문서가 생성된 애플리케이션 이름.


### Manager {#Manager}
```
public static final int Manager
```


작성자 관리자 이름.


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


수정 번호.


### Subject {#Subject}
```
public static final int Subject
```


문서의 주제.


### Template {#Template}
```
public static final int Template
```


문서 템플릿 이름.


### Title {#Title}
```
public static final int Title
```


문서 제목.


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


총 편집 시간.


### Version {#Version}
```
public static final int Version
```


문서 버전.


### Description {#Description}
```
public static final int Description
```


문서 설명.


### Keywords {#Keywords}
```
public static final int Keywords
```


문서 키워드.


### ContentType {#ContentType}
```
public static final int ContentType
```


콘텐츠 유형.


### All {#All}
```
public static final int All
```


메타데이터 항목의 모든 유형.


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


선언된 모든 필터 유형을 포함하는 집합을 가져옵니다.


**Returns:**
java.util.Set<java.lang.String> - 선언된 모든 필터 유형을 포함하는 집합.

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


MetadataFiler의 값을 이름으로 가져옵니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | valueName | java.lang.String | MetadataFilter의 이름. |
|

**Returns:**
int - MetadataFiler의 값.

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


쉼표로 구분된 MetadataFilers 값 문자열을 정수로 구문 분석합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | values | java.lang.String | 쉼표로 구분된 MetadataFilers 값 문자열. |
|

**Returns:**
int - MetadataFilers의 값.

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


정수를 쉼표로 구분된 MetadataFilers 값 문자열로 저장합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | int | MetadataFiler의 값. |
|

**Returns:**
java.lang.String - 쉼표로 구분된 MetadataFiler 값 문자열.

