---
title: "RegionReplacementOptions"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili parameter warna dan area untuk penggantian wilayah gambar."
type: docs
weight: 29
url: /id/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

Mewakili parameter warna dan area untuk penggantian wilayah gambar. Lihat
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | Menginisialisasi instance baru dari kelas RegionReplacementOptions. |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | Menginisialisasi instance baru dari kelas RegionReplacementOptions yang ukurannya cocok dengan teks yang diberikan. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | Mendapatkan warna untuk mengisi area yang direduksi. |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | Mengatur warna untuk mengisi area yang direduksi. |
|
|  | [getSize()](#getSize--) | Mendapatkan persegi panjang dengan lebar dan tinggi. |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | Mengatur persegi panjang dengan lebar dan tinggi. |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


Menginisialisasi instance baru dari kelas RegionReplacementOptions.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Warna untuk mengisi area |
|
|  | ukuran | java.awt.Dimension | Ukuran area terisi |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


Menginisialisasi instance baru dari kelas RegionReplacementOptions yang ukurannya cocok dengan teks yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Warna untuk mengisi area |
|
|  | font | java.awt.Font | Font teks yang diharapkan |
|
|  | expectedText | java.lang.String | Teks yang diharapkan |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


Mendapatkan warna untuk mengisi area yang direduksi.


**Returns:**
java.awt.Color - Warna untuk mengisi area yang disensor.

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


Mengatur warna untuk mengisi area yang direduksi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.awt.Color | Warna untuk mengisi area yang disensor. |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


Mendapatkan persegi panjang dengan lebar dan tinggi.


**Returns:**
java.awt.Dimension - Persegi panjang dengan lebar dan tinggi.

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


Mengatur persegi panjang dengan lebar dan tinggi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.awt.Dimension | Persegi panjang dengan lebar dan tinggi. |
|

