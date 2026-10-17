---
title: "RecognizedImage"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل النص المستخرج من صورة نتيجة عملية التعرف عليها."
type: docs
weight: 13
url: /ar/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

يمثل النص المستخرج من صورة نتيجة عملية التعرف عليها.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | يُنشئ مثيلاً جديدًا للفئة باستخدام مجموعة من السطور المعترف بها. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getText()](#getText--) | يحصل على المكافئ النصي للنص المُنظم. |
|
|  | [getLines()](#getLines--) | يحصل على سطور النص، مع قطعها، المعترف بها داخل المستند. |
|
|  | [toString()](#toString--) | يحصل على المكافئ النصي للنص المُنظم. |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


يُنشئ مثيلاً جديدًا للفئة باستخدام مجموعة من السطور المعترف بها.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | IEnumerable (مثل قائمة أو مصفوفة) من السطور المعترف بها |
|

### getText() {#getText--}
```
public final String getText()
```


يحصل على المكافئ النصي للنص المُنظم.


**Returns:**
java.lang.String - المكافئ النصي للنص المُنظم.

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


يحصل على سطور النص، مع قطعها، المعترف بها داخل المستند.


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - سطور النص، مع قطعها، المعترف بها داخل المستند.

### toString() {#toString--}
```
public String toString()
```


يحصل على المكافئ النصي للنص المُنظم.


**Returns:**
java.lang.String - النص المعترف به

