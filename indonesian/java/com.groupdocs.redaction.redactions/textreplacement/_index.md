---
title: "TextReplacement"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili informasi penggantian tekstual."
type: docs
weight: 33
url: /id/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

Mewakili informasi penggantian tekstual.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | Menginisialisasi instance baru dari kelas TextReplacement. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getIndex()](#getIndex--) | Mendapatkan indeks teks yang cocok dalam string sumber. |
|
|  | [getOriginalText()](#getOriginalText--) | Mendapatkan string asli yang cocok. |
|
|  | [getReplacement()](#getReplacement--) | Mendapatkan string, menggantikan OriginalText. |
|
|  | [toString()](#toString--) | Menyediakan deskripsi penggantian teks dan posisinya. |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


Menginisialisasi instance baru dari kelas TextReplacement.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indeks | int | Indeks teks yang cocok dalam string sumber |
|
|  | asli | java.lang.String | String yang cocok asli |
|
|  | penggantian | java.lang.String | String, menggantikan OriginalText dalam string sumber |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Mendapatkan indeks teks yang cocok dalam string sumber.


**Returns:**
int - Indeks teks yang cocok dalam string sumber.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Mendapatkan string asli yang cocok.


**Returns:**
java.lang.String - String yang cocok asli.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Mendapatkan string, menggantikan OriginalText.


**Returns:**
java.lang.String - String, menggantikan OriginalText.

### toString() {#toString--}
```
public String toString()
```


Menyediakan deskripsi penggantian teks dan posisinya.


**Returns:**
java.lang.String - Deskripsi penggantian

