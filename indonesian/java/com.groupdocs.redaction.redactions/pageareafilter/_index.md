---
title: "PageAreaFilter"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili filter redaksi yang mengatur area dalam sebuah halaman dokumen untuk menerapkan redaksi."
type: docs
weight: 22
url: /id/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

Mewakili filter redaksi, mengatur area dalam sebuah halaman dokumen untuk menerapkan redaksi.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | Menginisialisasi instance baru dari kelas PageAreaFilter untuk meredaksi area tertentu. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Mendapatkan persegi panjang (posisi kiri-atas dan ukuran area) pada sebuah halaman. |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | Memeriksa apakah area filter ini berpotongan dengan persegi panjang yang diberikan. |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


Menginisialisasi instance baru dari kelas PageAreaFilter untuk meredaksi area tertentu.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Koordinat area kiri-atas |
|
|  | ukuran | java.awt.Dimension | Ukuran dan warna area |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Mendapatkan persegi panjang (posisi kiri-atas dan ukuran area) pada sebuah halaman.


**Returns:**
java.awt.Rectangle - Persegi panjang (posisi kiri-atas dan ukuran area) pada sebuah halaman.

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


Memeriksa apakah area filter ini berpotongan dengan persegi panjang yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | persegi panjang | java.awt.Rectangle | Persegi panjang untuk diperiksa |
|

**Returns:**
boolean - true, jika area filter ini berpotongan

