---
title: "CustomRedactionContext"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يوفر بيانات الإدخال لـ ."
type: docs
weight: 13
url: /ar/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

يوفر بيانات الإدخال لـ [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | يحصل على رقم الصفحة للجزء المتطابق، إذا كان متاحًا. |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | يضبط رقم الصفحة للجزء المتطابق. |
|
|  | [getText()](#getText--) | يحصل على النص المتطابق للتعتيم. |
|
|  | [setText(String value)](#setText-java.lang.String-) | يضبط النص المتطابق للتعتيم. |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


يحصل على رقم الصفحة للجزء المتطابق، إذا كان متاحًا.


**Returns:**
int - رقم الصفحة، أو قيمة محددة حسب التنسيق إذا لم يكن رقم الصفحة معروفًا.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


يضبط رقم الصفحة للجزء المتطابق.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | int | رقم الصفحة. |
|

### getText() {#getText--}
```
public final String getText()
```


يحصل على النص المتطابق للتعتيم.


**Returns:**
java.lang.String - النص المتطابق.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


يضبط النص المتطابق للتعتيم.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.lang.String | النص المتطابق. |
|

