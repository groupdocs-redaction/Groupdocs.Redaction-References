---
title: "RedactionResult"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "가림 처리 작업의 결과를 나타냅니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

가림 처리 작업의 결과를 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getStatus()](#getStatus--) | 실행 상태를 가져옵니다. |
|
|  | [getErrorMessage()](#getErrorMessage--) | 진단을 위한 오류 메시지를 가져옵니다. |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | Skipped 상태와 함께 RedactionResult 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [partial(String description)](#partial-java.lang.String-) | PartiallyApplied 상태와 함께 RedactionResult 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [failed(String description)](#failed-java.lang.String-) | Failed 상태와 함께 RedactionResult 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [successful()](#successful--) | Applied (successful) 상태와 함께 RedactionResult 클래스의 새 인스턴스를 초기화합니다. |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


실행 상태를 가져옵니다.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


진단을 위한 오류 메시지를 가져옵니다.


**Returns:**
java.lang.String - 진단을 위한 오류 메시지.

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


Skipped 상태와 함께 RedactionResult 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 설명 | java.lang.String | 작업이 건너뛰어진 이유 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


PartiallyApplied 상태와 함께 RedactionResult 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 설명 | java.lang.String | 작업이 완전히 적용되지 않은 이유 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


Failed 상태와 함께 RedactionResult 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 설명 | java.lang.String | 실패 또는 예외 세부 정보 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


Applied (successful) 상태와 함께 RedactionResult 클래스의 새 인스턴스를 초기화합니다.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

