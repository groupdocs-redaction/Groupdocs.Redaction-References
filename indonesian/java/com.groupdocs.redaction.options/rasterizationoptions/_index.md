---
title: "RasterizationOptions"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Menyediakan opsi untuk mengonversi file menjadi PDF."
type: docs
weight: 12
url: /id/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

Menyediakan opsi untuk mengonversi file menjadi PDF.

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | Menginisialisasi instance baru. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Mendapatkan nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Mengatur nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF. |
|
|  | [getPageIndex()](#getPageIndex--) | Mendapatkan indeks halaman pertama (berbasis 0) untuk dikonversi menjadi PDF. |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | Mengatur indeks halaman pertama (berbasis 0) untuk dikonversi menjadi PDF. |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | Mendapatkan nilai yang menunjukkan apakah properti PageIndex telah diubah (diset) setelah inisialisasinya. |
|
|  | [getPageCount()](#getPageCount--) | Mendapatkan jumlah halaman yang akan dikonversi menjadi PDF. |
|
|  | [setPageCount(int value)](#setPageCount-int-) | Mengatur jumlah halaman yang akan dikonversi menjadi PDF. |
|
|  | [isPageCountSet()](#isPageCountSet--) | Mendapatkan nilai yang menunjukkan apakah properti PageCount telah diubah (diset) setelah inisialisasinya. |
|
|  | [getCompliance()](#getCompliance--) | Mendapatkan tingkat Kepatuhan PDF. |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | Mengatur tingkat Kepatuhan PDF. |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | Mendapatkan indikator, yang bernilai true jika opsi rasterisasi lanjutan telah diset. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan yang akan diterapkan. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan yang akan diterapkan. |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


Menginisialisasi instance baru.


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


Mendapatkan nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF. TRUE secara default, set ke FALSE untuk menghindari rasterisasi.


**Returns:**
boolean - Nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF. TRUE secara default, set ke FALSE untuk menghindari rasterisasi.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


Mengatur nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF. TRUE secara default, set ke FALSE untuk menghindari rasterisasi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF. TRUE secara default, set ke FALSE untuk menghindari rasterisasi. |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Mendapatkan indeks halaman pertama (berbasis 0) untuk dikonversi menjadi PDF.


**Returns:**
int - Indeks halaman pertama (berbasis 0) yang akan dikonversi menjadi PDF.

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Mengatur indeks halaman pertama (berbasis 0) untuk dikonversi menjadi PDF.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Indeks halaman pertama (berbasis 0) yang akan dikonversi menjadi PDF. |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


Mendapatkan nilai yang menunjukkan apakah properti PageIndex telah diubah (diset) setelah inisialisasinya.


**Returns:**
boolean - Nilai yang menunjukkan apakah properti PageIndex telah diubah (diset) setelah inisialisasinya.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Mendapatkan jumlah halaman yang akan dikonversi menjadi PDF.


**Returns:**
int - Jumlah halaman yang akan dikonversi menjadi PDF.

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Mengatur jumlah halaman yang akan dikonversi menjadi PDF.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah halaman yang akan dikonversi menjadi PDF. |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


Mendapatkan nilai yang menunjukkan apakah properti PageCount telah diubah (diset) setelah inisialisasinya.


**Returns:**
boolean - Nilai yang menunjukkan apakah properti PageCount telah diubah (diset) setelah inisialisasinya.

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


Mendapatkan tingkat Kepatuhan PDF.


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


Mengatur tingkat Kepatuhan PDF.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | Tingkat Kepatuhan PDF. |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


Mendapatkan indikator, yang bernilai true jika opsi rasterisasi lanjutan telah diset.


**Returns:**
boolean - Indikator, yang bernilai true jika opsi rasterisasi lanjutan telah diset.

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan yang akan diterapkan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Memberikan informasi tentang tipe efek yang dipilih (grayscale, border, dll.) |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan yang akan diterapkan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Memberikan informasi tentang tipe efek yang dipilih (grayscale, border, dll.) |
|
|  | parameter | java.util.HashMap<java.lang.String,java.lang.String> | Parameter untuk efek yang diberikan, seperti sudut rotasi |
|

