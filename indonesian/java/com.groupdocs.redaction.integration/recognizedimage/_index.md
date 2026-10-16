---
title: "RecognizedImage"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili teks yang diekstrak dari gambar sebagai hasil dari proses pengenalan."
type: docs
weight: 13
url: /id/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

Mewakili teks, diekstrak dari gambar sebagai hasil proses pengenalan.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | Menginisialisasi instance baru dari kelas, menggunakan sekumpulan baris yang dikenali. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getText()](#getText--) | Mendapatkan padanan teks dari teks terstruktur. |
|
|  | [getLines()](#getLines--) | Mendapatkan baris teks, beserta fragmennya, yang dikenali dalam dokumen. |
|
|  | [toString()](#toString--) | Mendapatkan padanan teks dari teks terstruktur. |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


Menginisialisasi instance baru dari kelas, menggunakan sekumpulan baris yang dikenali.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | sebuah IEnumerable (misalnya daftar atau array) dari baris yang dikenali |
|

### getText() {#getText--}
```
public final String getText()
```


Mendapatkan padanan teks dari teks terstruktur.


**Returns:**
java.lang.String - Padanan teks dari teks terstruktur.

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


Mendapatkan baris teks, beserta fragmennya, yang dikenali dalam dokumen.


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - Baris teks, beserta fragmennya, yang dikenali dalam dokumen.

### toString() {#toString--}
```
public String toString()
```


Mendapatkan padanan teks dari teks terstruktur.


**Returns:**
java.lang.String - Teks yang dikenali

