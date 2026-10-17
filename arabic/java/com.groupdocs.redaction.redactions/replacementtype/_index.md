---
title: "ReplacementType"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل نوعًا من الاستبدال للنص المطابق."
type: docs
weight: 38
url: /ar/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

يمثل نوعًا من الاستبدال للنص المطابق.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | يستبدل النص المطابق بسلسلة أخرى، على سبيل المثال. |
|
|  | [DrawBox](#DrawBox) | يرسم مستطيلًا بلون محدد (أسود افتراضيًا) بدلاً من النص المشفر. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


يستبدل النص المطابق بسلسلة أخرى، على سبيل المثال رمز الإعفاء.


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


يرسم مستطيلًا بلون محدد (أسود افتراضيًا) بدلاً من النص المشفر.


### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
