---
title: "RedactionStatus"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل حالة إكمال التمويه."
type: docs
weight: 20
url: /ar/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

يمثل حالة إكمال التمويه.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [Applied](#Applied) | تم تطبيق Redaction بالكامل وبنجاح. |
|
|  | [PartiallyApplied](#PartiallyApplied) | تم تطبيق Redaction فقط على جزء من التطابقات. |
|
|  | [Skipped](#Skipped) | تم تخطي Redaction (لم يتم تطبيقه). |
|
|  | [Failed](#Failed) | فشل Redaction مع استثناء. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


تم تطبيق Redaction بالكامل وبنجاح.


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


تم تطبيق Redaction فقط على جزء من التطابقات.


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


تم تخطي Redaction (لم يتم تطبيقه).


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


فشل Redaction مع استثناء.


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
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
