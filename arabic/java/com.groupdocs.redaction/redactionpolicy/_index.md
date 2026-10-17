---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل سياسة تنقية تحتوي على مجموعة من عمليات الحذف المحددة لتطبيقها."
type: docs
weight: 14
url: /ar/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

يمثل سياسة التطهير، تحتوي على مجموعة من عمليات التمويه المحددة لتطبيقها.

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | ينشئ مثالًا جديدًا لسياسة الحذف. |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | ينشئ مثالًا جديدًا لسياسة الحذف مع قائمة محددة من عمليات الحذف. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | يحصل على مصفوفة مُكوَّنة بالكامل |
الحذف
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | يحمّل مثالًا من |
RedactionPolicy
من مسار ملف.
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | يحمّل مثالًا من |
RedactionPolicy
من تدفق.
|
|  | [save(String filePath)](#save-java.lang.String-) | يحفظ سياسة الحذف إلى ملف. |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | يحفظ سياسة الحذف إلى تدفق. |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


ينشئ مثالًا جديدًا لسياسة الحذف.


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


ينشئ مثالًا جديدًا لسياسة الحذف مع قائمة محددة من عمليات الحذف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | مصفوفة من عمليات الحذف للسياسة |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


يحصل على مصفوفة مُكوَّنة بالكامل
الحذف
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - مصفوفة من الفئات المشتقة من Redaction المُكوَّنة بالكامل.

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


يحمّل مثالًا من
RedactionPolicy
من مسار ملف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى ملف XML |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


يحمّل مثالًا من
RedactionPolicy
من تدفق.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | input | java.io.InputStream | تدفق يحتوي على تكوين XML |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


يحفظ سياسة الحذف إلى ملف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى الملف. |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


يحفظ سياسة الحذف إلى تدفق.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | output | java.io.OutputStream | التدفق الهدف لحفظ السياسة |
|

