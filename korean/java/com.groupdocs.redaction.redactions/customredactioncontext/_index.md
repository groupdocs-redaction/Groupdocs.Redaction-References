---
title: "CustomRedactionContext"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "입력 데이터를 제공합니다 ."
type: docs
weight: 13
url: /ko/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

입력 데이터를 제공합니다 [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | 일치하는 조각의 페이지 번호를 가져옵니다, 가능한 경우. |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | 일치하는 조각의 페이지 번호를 설정합니다. |
|
|  | [getText()](#getText--) | 삭제를 위해 일치한 텍스트를 가져옵니다. |
|
|  | [setText(String value)](#setText-java.lang.String-) | 삭제를 위해 일치한 텍스트를 설정합니다. |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


일치하는 조각의 페이지 번호를 가져옵니다, 가능한 경우.


**Returns:**
int - 페이지 번호, 또는 페이지를 알 수 없는 경우 형식별 값.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


일치하는 조각의 페이지 번호를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | int | 페이지 번호. |
|

### getText() {#getText--}
```
public final String getText()
```


삭제를 위해 일치한 텍스트를 가져옵니다.


**Returns:**
java.lang.String - 일치한 텍스트.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


삭제를 위해 일치한 텍스트를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 일치한 텍스트. |
|

