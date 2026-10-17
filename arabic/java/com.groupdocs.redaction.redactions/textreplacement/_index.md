---
title: "TextReplacement"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل معلومات استبدال نصية."
type: docs
weight: 33
url: /ar/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

يمثل معلومات استبدال نصية.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | يُهيئ مثيلًا جديدًا من الفئة TextReplacement. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getIndex()](#getIndex--) | يحصل على فهرس النص المتطابق داخل سلسلة المصدر. |
|
|  | [getOriginalText()](#getOriginalText--) | يحصل على السلسلة المتطابقة الأصلية. |
|
|  | [getReplacement()](#getReplacement--) | يحصل على السلسلة، مستبدلاً OriginalText. |
|
|  | [toString()](#toString--) | يوفر وصف استبدال النص وموقعه. |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


يُهيئ مثيلًا جديدًا من الفئة TextReplacement.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | فهرس | int | فهرس النص المطابق داخل السلسلة المصدر |
|
|  | الأصلي | java.lang.String | السلسلة المطابقة الأصلية |
|
|  | استبدال | java.lang.String | سلسلة، تستبدل OriginalText في السلسلة المصدر |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


يحصل على فهرس النص المتطابق داخل سلسلة المصدر.


**Returns:**
int - فهرس النص المطابق داخل السلسلة المصدر.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


يحصل على السلسلة المتطابقة الأصلية.


**Returns:**
java.lang.String - السلسلة المطابقة الأصلية.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


يحصل على السلسلة، مستبدلاً OriginalText.


**Returns:**
java.lang.String - السلسلة، مستبدلة OriginalText.

### toString() {#toString--}
```
public String toString()
```


يوفر وصف استبدال النص وموقعه.


**Returns:**
java.lang.String - وصف الاستبدال

