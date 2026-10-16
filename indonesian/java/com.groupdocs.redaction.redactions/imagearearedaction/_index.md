---
title: "ImageAreaRedaction"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili redaksi yang menempatkan persegi panjang berwarna di area tertentu dari dokumen gambar."
type: docs
weight: 18
url: /id/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

Mewakili redaksi yang menempatkan persegi panjang berwarna di area tertentu dari dokumen gambar.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Menginisialisasi instance baru dari kelas ImageAreaRedaction untuk menyensor ukuran area tertentu. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getOptions()](#getOptions--) | Mendapatkan |
RegionReplacementOptions
opsi dengan parameter warna dan area.
|
|  | [getTopLeft()](#getTopLeft--) | Mendapatkan posisi kiri-atas area yang akan dihapus |
|
|  | [getDescription()](#getDescription--) | Mengembalikan string yang menggambarkan redaksi dan parameternya. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Menerapkan redaksi pada instance format yang diberikan. |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


Menginisialisasi instance baru dari kelas ImageAreaRedaction untuk menyensor ukuran area tertentu.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Koordinat area kiri-atas |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Ukuran dan warna area |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


Mendapatkan
RegionReplacementOptions
opsi dengan parameter warna dan area.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


Mendapatkan posisi kiri-atas area yang akan dihapus


**Returns:**
java.awt.Point - Posisi kiri-atas area yang akan dihapus

### getDescription() {#getDescription--}
```
public String getDescription()
```


Mengembalikan string yang menggambarkan redaksi dan parameternya.


**Returns:**
java.lang.String - Teks, yang berisi nama redaksi dan parameter.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Menerapkan redaksi pada instance format yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Sebuah instance dokumen untuk menerapkan redaksi |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

