---
title: "TextLine"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili satu baris teks yang diekstrak oleh mesin OCR dari sebuah gambar."
type: docs
weight: 16
url: /id/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

Mewakili baris teks, diekstrak oleh mesin OCR dari gambar.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | Menginisialisasi instance baru dari baris teks, yang diekstrak oleh mesin OCR dari sebuah gambar. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFragments()](#getFragments--) | Mendapatkan array fragmen teks, seperti simbol dan kata, yang dikenali dalam baris. |
|
|  | [toString()](#toString--) | Mengembalikan konten tekstual dari baris teks yang dikenali. |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


Menginisialisasi instance baru dari baris teks, yang diekstrak oleh mesin OCR dari sebuah gambar.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | set awal fragmen teks |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


Mendapatkan array fragmen teks, seperti simbol dan kata, yang dikenali dalam baris.


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - Array fragmen teks, seperti simbol dan kata, yang dikenali dalam baris.

### toString() {#toString--}
```
public String toString()
```


Mengembalikan konten tekstual dari baris teks yang dikenali.


**Returns:**
java.lang.String - konten tekstual dari baris teks yang dikenali

