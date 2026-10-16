---
title: "RedactionStatus"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "가림 처리 완료 상태를 나타냅니다."
type: docs
weight: 20
url: /ko/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

가림 처리 완료 상태를 나타냅니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [Applied](#Applied) | Redaction이 완전하고 성공적으로 적용되었습니다. |
|
|  | [PartiallyApplied](#PartiallyApplied) | Redaction이 일치 항목의 일부에만 적용되었습니다. |
|
|  | [Skipped](#Skipped) | Redaction이 건너뛰어졌습니다 (적용되지 않음). |
|
|  | [Failed](#Failed) | Redaction이 예외와 함께 실패했습니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


Redaction이 완전하고 성공적으로 적용되었습니다.


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


Redaction이 일치 항목의 일부에만 적용되었습니다.


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


Redaction이 건너뛰어졌습니다 (적용되지 않음).


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


Redaction이 예외와 함께 실패했습니다.


### values() {#values--}
```
public static RedactionStatus[] values()
```




**Returns:**
com.groupdocs.redaction.RedactionStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionStatus valueOf(String name)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
