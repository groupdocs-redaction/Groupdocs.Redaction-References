---
title: "WordProcessingComplianceLevel"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "워드 프로세싱 문서에 대한 OOXML 호환성 수준."
type: docs
weight: 22
url: /ko/java/com.groupdocs.redaction.options/wordprocessingcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum WordProcessingComplianceLevel extends Enum<WordProcessingComplianceLevel>
```

워드 프로세싱 문서에 대한 OOXML 준수 수준입니다. Strict는 Ecma가 아니라 Transitional으로만 다운그레이드될 수 있습니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [Ecma](#Ecma) | ECMA-376 1st Edition, 2006. |
|
|  | [Transitional](#Transitional) | ISO/IEC 29500:2008 Transitional. |
|
|  | [Strict](#Strict) | ISO/IEC 29500:2008 Strict. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ecma {#Ecma}
```
public static final WordProcessingComplianceLevel Ecma
```


ECMA-376 1st Edition, 2006.


### Transitional {#Transitional}
```
public static final WordProcessingComplianceLevel Transitional
```


ISO/IEC 29500:2008 Transitional.


### Strict {#Strict}
```
public static final WordProcessingComplianceLevel Strict
```


ISO/IEC 29500:2008 Strict.


### values() {#values--}
```
public static WordProcessingComplianceLevel[] values()
```




**Returns:**
com.groupdocs.redaction.options.WordProcessingComplianceLevel[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static WordProcessingComplianceLevel valueOf(String name)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
