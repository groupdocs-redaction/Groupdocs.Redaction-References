---
title: "RedactableImage"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Menyediakan antarmuka untuk semua operasi redaksi gambar raster."
type: docs
weight: 14
url: /id/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

Menyediakan antarmuka untuk semua operasi redaksi gambar raster.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | Membuat sebuah instance baru menggunakan objek, yang mengimplementasikan |
IImageFormatInstance
antarmuka.
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | Membuat sebuah instance baru menggunakan objek, yang mengimplementasikan |
IMultipleAreaRedactable
antarmuka.
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | Mengambil aliran dengan konten gambar sebenarnya. |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Menyunting beberapa area gambar sekaligus dengan warna yang sama. |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Mengganti area pada titik yang diberikan dengan persegi panjang berwarna dan ukuran tertentu. |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


Membuat sebuah instance baru menggunakan objek, yang mengimplementasikan
IImageFormatInstance
antarmuka.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | Sebuah instance, yang mengimplementasikan antarmuka IImageFormatInstance |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


Membuat sebuah instance baru menggunakan objek, yang mengimplementasikan
IMultipleAreaRedactable
antarmuka.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | Sebuah instance, yang mengimplementasikan antarmuka IMultipleAreaRedactable |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


Mengambil aliran dengan konten gambar sebenarnya.


**Returns:**
java.io.InputStream - Aliran, yang berisi data gambar

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


Menyunting beberapa area gambar sekaligus dengan warna yang sama.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | persegi panjang | java.awt.Rectangle[] | Sebuah array area persegi panjang |
|
|  | boxColor | java.awt.Color | Warna untuk mengisi area |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Mengganti area pada titik yang diberikan dengan persegi panjang berwarna dan ukuran tertentu.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Koordinat sudut kiri atas area yang diisi |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Pengaturan warna dan ukuran |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

