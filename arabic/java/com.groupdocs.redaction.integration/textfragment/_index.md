---
title: "TextFragment"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل جزءًا من النص المعترف به مثل الكلمة أو الرمز وما إلى ذلك المستخرج بواسطة محرك OCR."
type: docs
weight: 15
url: /ar/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

يمثل جزءًا من النص المُعترف به (كلمة، رمز، إلخ)، مستخرجًا بواسطة محرك OCR.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | ينشئ نسخة جديدة من جزء النص المعترف به. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getText()](#getText--) | يحصل على المحتوى النصي للمقطع النصي المعترف به. |
|
|  | [getRectangle()](#getRectangle--) | يحصل على المستطيل المحيط بالمقطع النصي المعترف به. |
|
|  | [toString()](#toString--) | يعيد المحتوى النصي للمقطع النصي المعترف به. |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


ينشئ نسخة جديدة من جزء النص المعترف به.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | نص | java.lang.String | المحتوى النصي للمقطع النصي المعترف به |
|
|  | rectangle | java.awt.Rectangle | المستطيل المحيط بالمقطع النصي المعترف به |
|

### getText() {#getText--}
```
public final String getText()
```


يحصل على المحتوى النصي للمقطع النصي المعترف به.


**Returns:**
java.lang.String - محتوى نصي للمقطع النصي المعترف به.

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


يحصل على المستطيل المحيط بالمقطع النصي المعترف به.


**Returns:**
java.awt.Rectangle - مستطيل محيط بالمقطع النصي المعترف به.

### toString() {#toString--}
```
public String toString()
```


يعيد المحتوى النصي للمقطع النصي المعترف به.


**Returns:**
java.lang.String - المحتوى النصي للمقطع النصي المعترف به

