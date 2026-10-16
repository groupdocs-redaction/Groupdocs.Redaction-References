---
title: "TextFragment"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili bagian dari teks yang dikenali, kata, simbol, dll yang diekstrak oleh mesin OCR."
type: docs
weight: 15
url: /id/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

Mewakili bagian dari teks yang dikenali (kata, simbol, dll), diekstrak oleh mesin OCR.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | Menginisialisasi instance baru dari fragmen teks yang dikenali. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getText()](#getText--) | Mendapatkan konten tekstual dari fragmen teks yang dikenali. |
|
|  | [getRectangle()](#getRectangle--) | Mendapatkan persegi panjang pembatas dari fragmen teks yang dikenali. |
|
|  | [toString()](#toString--) | Mengembalikan konten tekstual dari fragmen teks yang dikenali. |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


Menginisialisasi instance baru dari fragmen teks yang dikenali.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | teks | java.lang.String | konten tekstual dari fragmen teks yang dikenali |
|
|  | persegi panjang | java.awt.Rectangle | persegi panjang pembatas dari fragmen teks yang dikenali |
|

### getText() {#getText--}
```
public final String getText()
```


Mendapatkan konten tekstual dari fragmen teks yang dikenali.


**Returns:**
java.lang.String - Konten tekstual dari fragmen teks yang dikenali.

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Mendapatkan persegi panjang pembatas dari fragmen teks yang dikenali.


**Returns:**
java.awt.Rectangle - Persegi panjang pembatas dari fragmen teks yang dikenali.

### toString() {#toString--}
```
public String toString()
```


Mengembalikan konten tekstual dari fragmen teks yang dikenali.


**Returns:**
java.lang.String - konten tekstual dari fragmen teks yang dikenali

