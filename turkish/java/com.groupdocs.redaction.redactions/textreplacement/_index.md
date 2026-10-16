---
title: "TextReplacement"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Metinsel bir değiştirme bilgisini temsil eder."
type: docs
weight: 33
url: /tr/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

Metinsel bir değiştirme bilgisini temsil eder.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | TextReplacement sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getIndex()](#getIndex--) | Kaynak dizede eşleşen metnin indeksini alır. |
|
|  | [getOriginalText()](#getOriginalText--) | Orijinal eşleşen dizeyi alır. |
|
|  | [getReplacement()](#getReplacement--) | OriginalText'i değiştiren dizeyi alır. |
|
|  | [toString()](#toString--) | Metin değiştirme açıklamasını ve konumunu sağlar. |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


TextReplacement sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indeks | int | Kaynak dizede eşleşen metnin indeksi |
|
|  | orijinal | java.lang.String | Orijinal eşleşen dize |
|
|  | değiştirme | java.lang.String | Kaynak dizede OriginalText'i değiştiren dize |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Kaynak dizede eşleşen metnin indeksini alır.


**Returns:**
int - Kaynak dizede eşleşen metnin indeksi.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Orijinal eşleşen dizeyi alır.


**Returns:**
java.lang.String - Orijinal eşleşen dize.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


OriginalText'i değiştiren dizeyi alır.


**Returns:**
java.lang.String - OriginalText'i değiştiren dize.

### toString() {#toString--}
```
public String toString()
```


Metin değiştirme açıklamasını ve konumunu sağlar.


**Returns:**
java.lang.String - Değiştirme açıklaması

