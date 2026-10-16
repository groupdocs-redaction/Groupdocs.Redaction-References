---
title: "CustomRedactionResult"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل نتيجة تم إرجاعها بواسطة ."
type: docs
weight: 14
url: /ar/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

يمثل نتيجة تم إرجاعها بواسطة [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getApply()](#getApply--) | يحصل على قيمة تشير إلى ما إذا كان يجب تطبيق الاستبدال. |
|
|  | [setApply(boolean value)](#setApply-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تطبيق الاستبدال. |
|
|  | [getText()](#getText--) | يحصل على نص الاستبدال المستخدم عندما يكون #getApply().getApply() |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | يضبط نص الاستبدال المستخدم عندما يكون #getApply().getApply() |
true
.
|
### CustomRedactionResult() {#CustomRedactionResult--}
```
public CustomRedactionResult()
```


### getApply() {#getApply--}
```
public final boolean getApply()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تطبيق الاستبدال.


**Returns:**
boolean -  true  لاستبدال النص المتطابق بـ #getText().getText(); وإلا،  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تطبيق الاستبدال.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | boolean | true  لتطبيق الاستبدال; وإلا،  false . |
|

### getText() {#getText--}
```
public final String getText()
```


يحصل على نص الاستبدال المستخدم عندما يكون #getApply().getApply()
true
.


**Returns:**
java.lang.String - نص الاستبدال.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


يضبط نص الاستبدال المستخدم عندما يكون #getApply().getApply()
true
.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.lang.String | نص الاستبدال. |
|

