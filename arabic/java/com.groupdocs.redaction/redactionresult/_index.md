---
title: "RedactionResult"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل نتيجة عملية التمويه."
type: docs
weight: 15
url: /ar/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

يمثل نتيجة عملية التمويه.

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getStatus()](#getStatus--) | يحصل على حالة التنفيذ. |
|
|  | [getErrorMessage()](#getErrorMessage--) | يحصل على رسالة الخطأ للتشخيص. |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة RedactionResult بالحالة Skipped. |
|
|  | [partial(String description)](#partial-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة RedactionResult بالحالة PartiallyApplied. |
|
|  | [failed(String description)](#failed-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة RedactionResult بالحالة Failed. |
|
|  | [successful()](#successful--) | ينشئ مثيلاً جديداً من الفئة RedactionResult بالحالة Applied (ناجحة). |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


يحصل على حالة التنفيذ.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


يحصل على رسالة الخطأ للتشخيص.


**Returns:**
java.lang.String - رسالة الخطأ للتشخيص.

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


ينشئ مثيلاً جديداً من الفئة RedactionResult بالحالة Skipped.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | الوصف | java.lang.String | السبب في تخطي العملية |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


ينشئ مثيلاً جديداً من الفئة RedactionResult بالحالة PartiallyApplied.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | الوصف | java.lang.String | السبب في عدم تطبيق العملية بالكامل |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


ينشئ مثيلاً جديداً من الفئة RedactionResult بالحالة Failed.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | الوصف | java.lang.String | تفاصيل الفشل أو الاستثناء |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


ينشئ مثيلاً جديداً من الفئة RedactionResult بالحالة Applied (ناجحة).


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

