---
title: "WordProcessingComplianceLevel"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "مستويات توافق OOXML لمستندات معالجة النصوص."
type: docs
weight: 22
url: /ar/java/com.groupdocs.redaction.options/wordprocessingcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum WordProcessingComplianceLevel extends Enum<WordProcessingComplianceLevel>
```

مستويات توافق OOXML لمستندات معالجة الكلمات. قد يتم تخفيض Strict إلى Transitional فقط، وليس إلى Ecma.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [Ecma](#Ecma) | ECMA-376 الطبعة الأولى، 2006. |
|
|  | [Transitional](#Transitional) | ISO/IEC 29500:2008 Transitional. |
|
|  | [Strict](#Strict) | ISO/IEC 29500:2008 Strict. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ecma {#Ecma}
```
public static final WordProcessingComplianceLevel Ecma
```


ECMA-376 الطبعة الأولى، 2006.


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
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
