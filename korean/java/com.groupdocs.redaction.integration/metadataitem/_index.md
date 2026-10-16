---
title: "MetadataItem"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "지원되는 모든 형식에 공통이며 메타데이터 편집에 사용되는 메타데이터 항목을 나타냅니다."
type: docs
weight: 12
url: /ko/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

모든 지원되는 형식에 공통이며 메타데이터 삭제에 사용되는 메타데이터 항목을 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | 문서에 표시되는 메타데이터 항목의 원래 이름을 가져옵니다. |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | 문서에 표시되는 메타데이터 항목의 원래 이름을 설정합니다. |
|
|  | [getCategory()](#getCategory--) | 예를 들어 임베디드 리소스 메타데이터 항목의 리소스 ID와 같은 메타데이터 항목의 카테고리를 가져옵니다. |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | 메타데이터 항목의 범주를 설정합니다. 예를 들어 포함된 리소스 메타데이터 항목의 리소스 ID가 있습니다. |
|
|  | [getFilter()](#getFilter--) | 값을 가져옵니다 |
MetadataFilters
, 이 메타데이터 항목에 할당되며 항목 필터링에 사용됩니다.
|
|  | [setFilter(int value)](#setFilter-int-) | 값을 설정합니다 |
MetadataFilters
, 이 메타데이터 항목에 할당되며 항목 필터링에 사용됩니다.
|
|  | [getValues()](#getValues--) | 메타데이터 항목 값을 가져옵니다. |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | 메타데이터 항목 값을 설정합니다. |
|
|  | [isCustom()](#isCustom--) | 이 항목이 사용자 지정인지 여부를 나타내는 값을 가져옵니다(문서 작성자가 추가함). |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | 이 항목이 사용자 지정인지 여부를 나타내는 값을 설정합니다(문서 작성자가 추가함). |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | 사전 키를 가져옵니다 , OriginalName 및 기타 데이터를 사용하여. |
|
|  | [createClone()](#createClone--) | 현재 인스턴스의 깊은 복제본을 생성합니다. |
|
|  | [getActualValue()](#getActualValue--) | 메타데이터 항목 값의 문자열 표현을 가져옵니다. |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


새 인스턴스를 초기화합니다.


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


문서에 표시되는 메타데이터 항목의 원래 이름을 가져옵니다.


**Returns:**
java.lang.String - 메타데이터 항목의 원래 이름, 문서에 표시되는 대로.

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


문서에 표시되는 메타데이터 항목의 원래 이름을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 메타데이터 항목의 원래 이름, 문서에 표시되는 대로. |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


예를 들어 임베디드 리소스 메타데이터 항목의 리소스 ID와 같은 메타데이터 항목의 카테고리를 가져옵니다.


**Returns:**
java.lang.String - 메타데이터 항목의 범주, 예를 들어 포함된 리소스 메타데이터 항목의 리소스 ID.

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


메타데이터 항목의 범주를 설정합니다. 예를 들어 포함된 리소스 메타데이터 항목의 리소스 ID가 있습니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 메타데이터 항목의 범주, 예를 들어 포함된 리소스 메타데이터 항목의 리소스 ID. |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


값을 가져옵니다
MetadataFilters
, 이 메타데이터 항목에 할당되며 항목 필터링에 사용됩니다.


**Returns:**
int - MetadataFilters 의 값, 이 메타데이터 항목에 할당되어 항목 필터링에 사용됩니다.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


값을 설정합니다
MetadataFilters
, 이 메타데이터 항목에 할당되며 항목 필터링에 사용됩니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | int | MetadataFilters 의 값, 이 메타데이터 항목에 할당되어 항목 필터링에 사용됩니다. |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


메타데이터 항목 값을 가져옵니다.


**Returns:**
java.util.List<java.lang.String> - 메타데이터 항목 값.

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


메타데이터 항목 값을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.util.List<java.lang.String> | 메타데이터 항목 값. |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


이 항목이 사용자 지정인지 여부를 나타내는 값을 가져옵니다(문서 작성자가 추가함).


**Returns:**
boolean - 이 항목이 사용자 지정인지 여부를 나타내는 값(문서 작성자가 추가함).

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


이 항목이 사용자 지정인지 여부를 나타내는 값을 설정합니다(문서 작성자가 추가함).


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 이 항목이 사용자 지정인지 여부를 나타내는 값(문서 작성자가 추가함). |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


사전 키를 가져옵니다 , OriginalName 및 기타 데이터를 사용하여.


**Returns:**
java.lang.String - OriginalName 및 기타 데이터를 사용하여 ,에 대한 사전 키.

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


현재 인스턴스의 깊은 복제본을 생성합니다.


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


메타데이터 항목 값의 문자열 표현을 가져옵니다.


**Returns:**
java.lang.String - 메타데이터 항목 값의 문자열 표현.

