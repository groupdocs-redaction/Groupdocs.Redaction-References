---
title: "CellFilter"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "CellColumnRedaction의 범위를 워크시트와 열로 제한하는 옵션을 제공합니다."
type: docs
weight: 12
url: /ko/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

범위 제한 옵션을 제공합니다.
CellColumnRedaction
워크시트와 열에 적용합니다.

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | 새 인스턴스를 초기화합니다. |
|
## 필드

| 필드 | 설명 |
| --- | --- |
|  | [NoIndex](#NoIndex) | 필터의 기본값을 나타내며, -1입니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | 워크시트 이름을 가져옵니다 (해당되는 경우). |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | 워크시트 이름을 설정합니다 (해당되는 경우). |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | 워크시트 인덱스를 가져옵니다 (0부터 시작). |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | 워크시트 인덱스를 설정합니다 (0부터 시작). |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | 해당 여부를 나타내는 값을 가져옵니다. |
WorkSheetIndex
설정되었는지 여부.
|
|  | [getColumnIndex()](#getColumnIndex--) | 열 인덱스(0 기반)를 가져옵니다. |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | 열 인덱스(0 기반)를 설정합니다. |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


새 인스턴스를 초기화합니다.


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


필터의 기본값을 나타내며, -1입니다.


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


워크시트 이름을 가져옵니다 (해당되는 경우).


**Returns:**
java.lang.String - 적용 가능한 경우 워크시트 이름.

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


워크시트 이름을 설정합니다 (해당되는 경우).


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 워크시트 이름(해당되는 경우). |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


워크시트 인덱스를 가져옵니다 (0부터 시작).


**Returns:**
int - 워크시트 인덱스(0 기반).

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


워크시트 인덱스를 설정합니다 (0부터 시작).


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | int | 워크시트 인덱스(0 기반). |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


해당 여부를 나타내는 값을 가져옵니다.
WorkSheetIndex
설정되었는지 여부.


**Returns:**
boolean - WorkSheetIndex가 설정되었는지 여부를 나타내는 값.

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


열 인덱스(0 기반)를 가져옵니다.


**Returns:**
int - 열 인덱스(0 기반).

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


열 인덱스(0 기반)를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | int | 열 인덱스(0 기반). |
|

