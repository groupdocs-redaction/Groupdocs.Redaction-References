---
title: "RedactionActionType"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل الإجراءات التي يمكن اتخاذها لتنفيذ الإزالة."
type: docs
weight: 37
url: /ar/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

يمثل الإجراءات التي يمكن اتخاذها لتنفيذ الإزالة.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [Replacement](#Replacement) | تم استبدال النص المحذوف بنص آخر أو تغطيته بكتلة. |
|
|  | [Cleanup](#Cleanup) | تمت إزالة البيانات، لكن يبقى كائن فارغ في المستند. |
|
|  | [Deletion](#Deletion) | تمت إزالة البيانات والهياكل المرتبطة من المستند. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


تم استبدال النص المحذوف بنص آخر أو تغطيته بكتلة.


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


تمت إزالة البيانات، لكن يبقى كائن فارغ في المستند.


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


تمت إزالة البيانات والهياكل المرتبطة من المستند.


### values() {#values--}
```
public static RedactionActionType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.RedactionActionType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionActionType valueOf(String name)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
