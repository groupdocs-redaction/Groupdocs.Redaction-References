---
title: "WordprocessingSaveOptions"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "خيارات حفظ معالجة النصوص."
type: docs
weight: 15
url: /ar/java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

خيارات حفظ معالجة النصوص.

## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getOoxmlCompliance()](#getOoxmlCompliance--) | امتثال OOXML لتطبيقه عند الحفظ. |
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


امتثال OOXML لتطبيقه عند الحفظ.  null  يحافظ على مستوى المستند الأصلي. لا يمكن حفظ Strict كـ Ecma مباشرةً؛ استخدم Transitional أولاً.


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

