---
title: "TextLine"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثّل سطر نص مستخرج بواسطة محرك OCR من صورة."
type: docs
weight: 16
url: /ar/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

يمثل سطرًا من النص، مستخرجًا بواسطة محرك OCR من صورة.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | يُنشئ نسخة جديدة من سطر نص، مستخرج بواسطة محرك OCR من صورة. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getFragments()](#getFragments--) | يحصل على مصفوفة من مقاطع النص، مثل الرموز والكلمات، المعترف بها في السطر. |
|
|  | [toString()](#toString--) | يعيد المحتوى النصي للسطر النصي المعترف به. |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


يُنشئ نسخة جديدة من سطر نص، مستخرج بواسطة محرك OCR من صورة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | مجموعة أولية من مقاطع النص |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


يحصل على مصفوفة من مقاطع النص، مثل الرموز والكلمات، المعترف بها في السطر.


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - مصفوفة من مقاطع النص، مثل الرموز والكلمات، المعترف بها في السطر.

### toString() {#toString--}
```
public String toString()
```


يعيد المحتوى النصي للسطر النصي المعترف به.


**Returns:**
java.lang.String - المحتوى النصي للسطر النصي المعترف به

