---
title: "WordprocessingSaveOptions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "워드 프로세싱 저장 옵션."
type: docs
weight: 15
url: /ko/java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

워드 프로세싱 저장 옵션.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getOoxmlCompliance()](#getOoxmlCompliance--) | 저장 시 적용할 OOXML 호환성. |
|
| [setOoxmlCompliance(WordProcessingComplianceLevel value)](#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-) |  |
### WordprocessingSaveOptions() {#WordprocessingSaveOptions--}
```
public WordprocessingSaveOptions()
```


### getOoxmlCompliance() {#getOoxmlCompliance--}
```
public final WordProcessingComplianceLevel getOoxmlCompliance()
```


저장 시 적용할 OOXML 호환성.  null  은 원본 문서 수준을 유지합니다. Strict는 직접 Ecma로 저장할 수 없으며, 먼저 Transitional을 사용하십시오.


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

