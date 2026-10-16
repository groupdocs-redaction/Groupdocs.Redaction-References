---
title: "RedactionActionType"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "삭제를 수행하기 위해 취할 수 있는 작업을 나타냅니다."
type: docs
weight: 37
url: /ko/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

삭제를 수행하기 위해 취할 수 있는 작업을 나타냅니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [Replacement](#Replacement) | 삭제된 텍스트는 다른 텍스트로 교체되었거나 블록으로 가려졌습니다. |
|
|  | [Cleanup](#Cleanup) | 데이터가 제거되었지만, 문서에 빈 객체가 남아 있습니다. |
|
|  | [Deletion](#Deletion) | 데이터와 관련 구조가 문서에서 제거되었습니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


삭제된 텍스트는 다른 텍스트로 교체되었거나 블록으로 가려졌습니다.


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


데이터가 제거되었지만, 문서에 빈 객체가 남아 있습니다.


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


데이터와 관련 구조가 문서에서 제거되었습니다.


### values() {#values--}
```
public static RedactionActionType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.RedactionActionType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionActionType valueOf(String name)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
