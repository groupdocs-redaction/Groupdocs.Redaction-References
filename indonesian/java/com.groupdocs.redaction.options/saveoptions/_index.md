---
title: "SaveOptions"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Menyediakan opsi untuk mengubah nama file output dan/atau mengonversi dokumen menjadi rasterisasi PDF berbasis gambar."
type: docs
weight: 14
url: /id/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

Menyediakan opsi untuk mengubah nama file output dan/atau mengonversi dokumen menjadi PDF berbasis gambar (rasterisasi).

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | Menginisialisasi instance baru dengan nilai default: rasterisasi ke PDF - false, tambahkan akhiran - false. |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | Menginisialisasi instance baru dengan parameter yang diberikan. |
|
## Bidang

| Bidang | Deskripsi |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | Mewakili nilai akhiran default, yaitu "Redacted". |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | Mendapatkan nilai yang menunjukkan apakah nama file perlu diubah sebelum disimpan. |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | Mengatur nilai yang menunjukkan apakah nama file perlu diubah sebelum disimpan. |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | Mendapatkan akhiran khusus untuk nama file output. |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | Mengatur akhiran khusus untuk nama file output. |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | Mendapatkan nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF. |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | Mengatur nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF. |
|
|  | [getRasterization()](#getRasterization--) | Mendapatkan pengaturan rasterisasi. |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | Opsi penyimpanan pengolah kata. |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


Menginisialisasi instance baru dengan nilai default: rasterisasi ke PDF - false, tambahkan akhiran - false.


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


Menginisialisasi instance baru dengan parameter yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | True, jika semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF |
|
|  | akhiran | java.lang.String | Teks ini akan ditambahkan ke akhir nama file, jika tidak kosong juga mengatur AddSuffix menjadi true |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


Mewakili nilai akhiran default, yaitu "Redacted".


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


Mendapatkan nilai yang menunjukkan apakah nama file perlu diubah sebelum disimpan. False secara default.


**Returns:**
boolean - Nilai yang menunjukkan apakah nama file perlu diubah sebelum disimpan. False secara default.

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


Mengatur nilai yang menunjukkan apakah nama file perlu diubah sebelum disimpan. False secara default.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah nama file perlu diubah sebelum disimpan. False secara default. |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


Mendapatkan akhiran khusus untuk nama file output. Jika tidak ditentukan,
SaveSuffix
konstanta akan digunakan.


**Returns:**
java.lang.String - Akhiran khusus untuk nama file output. Jika tidak ditentukan, konstanta SaveSuffix akan digunakan.

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


Mengatur akhiran khusus untuk nama file output. Jika tidak ditentukan,
SaveSuffix
konstanta akan digunakan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Sebuah akhiran khusus untuk nama file output. Jika tidak ditentukan, konstanta SaveSuffix akan digunakan. |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


Mendapatkan nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF.


**Returns:**
boolean - Nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF.

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


Mengatur nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF. |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


Mendapatkan pengaturan rasterisasi.


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


Opsi penyimpanan pengolah kata.


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
