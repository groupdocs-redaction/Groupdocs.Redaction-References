---
title: "ReplacementType"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "일치된 텍스트에 대한 교체 유형을 나타냅니다."
type: docs
weight: 38
url: /ko/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

일치된 텍스트에 대한 교체 유형을 나타냅니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | 일치하는 텍스트를 다른 문자열로 교체합니다, e.g. |
|
|  | [DrawBox](#DrawBox) | 특정 색(기본값은 검정)으로 사각형을 그려서 삭제된 텍스트 대신 표시합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


일치하는 텍스트를 다른 문자열로 교체합니다, e.g. 면제 코드.


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


특정 색(기본값은 검정)으로 사각형을 그려서 삭제된 텍스트 대신 표시합니다.


### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
