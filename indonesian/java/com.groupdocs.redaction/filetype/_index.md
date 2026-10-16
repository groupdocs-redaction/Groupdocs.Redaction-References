---
title: "FileType"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili tipe file."
type: docs
weight: 11
url: /id/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

Mewakili tipe file. Menyediakan metode untuk memperoleh daftar semua tipe file yang didukung oleh GroupDocs.Redaction, mendeteksi tipe file berdasarkan ekstensi, dll.

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Mendapatkan nama tipe file, misalnya "Microsoft Word Document". |
|
|  | [getExtension()](#getExtension--) | Mendapatkan akhiran nama file (termasuk titik "."), misalnya ".doc". |
|
|  | [getUnknown()](#getUnknown--) | Mewakili tipe file yang tidak diketahui. |
|
|  | [getTIF()](#getTIF--) | Tagged Image File (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Tagged Image File Format (.tiff) |
|
|  | [getJPG()](#getJPG--) | Gambar JPEG (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | Gambar JPEG (.jpeg) |
|
|  | [getPNG()](#getPNG--) | Grafik Jaringan Portabel (.png) |
|
|  | [getGIF()](#getGIF--) | Berkas Format Pertukaran Grafis (.gif) |
|
|  | [getBMP()](#getBMP--) | Berkas Gambar Bitmap (.bmp) |
|
|  | [getJP2()](#getJP2--) | Berkas Gambar Inti JPEG 2000 (.jp2) |
|
|  | [getHTM()](#getHTM--) | Berkas Bahasa Markah Hiperteks (.htm) |
|
|  | [getHTML()](#getHTML--) | Berkas Bahasa Markah Hiperteks (.html) |
|
|  | [getPDF()](#getPDF--) | Berkas Format Dokumen Portabel (.pdf) |
|
|  | [getPPT()](#getPPT--) | Presentasi PowerPoint (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | Presentasi PowerPoint Open XML (.pptx) |
|
|  | [getODP()](#getODP--) | Presentasi OpenDocument (.odp) |
|
|  | [getPOTX()](#getPOTX--) | Templat Presentasi PowerPoint Open XML (.potx) |
|
|  | [getPOTM()](#getPOTM--) | Templat Presentasi PowerPoint Open XML yang Mendukung Makro (.potm) |
|
|  | [getOTP()](#getOTP--) | Templat Presentasi OpenDocument (.otp) |
|
|  | [getXLS()](#getXLS--) | Lembar Kerja Excel (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Lembar Kerja Microsoft Excel Open XML (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Lembar Kerja Excel Open XML yang Mendukung Makro (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Lembar Kerja Biner Excel (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Templat Lembar Kerja Excel Open XML (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Templat Lembar Kerja Excel Open XML yang Mendukung Makro (.xltm) |
|
|  | [getXLT()](#getXLT--) | Templat Excel (.xlt) |
|
|  | [getCSV()](#getCSV--) | Berkas Nilai Dipisahkan Koma (.csv) |
|
|  | [getTSV()](#getTSV--) | Berkas Nilai Dipisahkan Tab (.tsv) |
|
|  | [getTAB()](#getTAB--) | Berkas Nilai Dipisahkan Tab (.tab) |
|
|  | [getODS()](#getODS--) | OpenDocument Spreadsheet (.ods) |
|
|  | [getOTS()](#getOTS--) | OpenDocument Spreadsheet Template (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Apple Numbers Spreadsheet (.numbers) |
|
|  | [getMD()](#getMD--) | File Dokumentasi Markdown (.md) |
|
|  | [getDOC()](#getDOC--) | Microsoft Word Document (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Microsoft Word Open XML Document (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Word Open XML Macro-Enabled Document (.docm) |
|
|  | [getDOT()](#getDOT--) | Word Document Template (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Word Open XML Document Template (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Word Open XML Macro-Enabled Document Template (.dotm) |
|
|  | [getRTF()](#getRTF--) | File Rich Text Format (.rtf) |
|
|  | [getTXT()](#getTXT--) | File Teks Biasa (.txt) |
|
|  | [getODT()](#getODT--) | OpenDocument Text Document (.odt) |
|
|  | [getOTT()](#getOTT--) | OpenDocument Document Template (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | Memetakan ekstensi file ke tipe file. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | Mengambil tipe file yang didukung |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | Menentukan apakah yang saat ini |
FileType
sama dengan yang ditentukan
FileType
objek.
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | Menentukan apakah yang saat ini |
FileType
sama dengan objek yang ditentukan.
|
|  | [hashCode()](#hashCode--) | Mengembalikan kode hash untuk yang saat ini |
FileType
objek.
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Menentukan apakah dua |
FileType
objek sama.
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Menentukan apakah dua |
FileType
objek tidak sama.
|
|  | [toString()](#toString--) | Mengembalikan string yang merepresentasikan objek saat ini. |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


Mendapatkan nama tipe file, misalnya "Microsoft Word Document".


**Returns:**
java.lang.String - Nama tipe file, misalnya "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


Mendapatkan akhiran nama file (termasuk titik "."), misalnya ".doc".


**Returns:**
java.lang.String - Akhiran nama file (termasuk titik "."), misalnya ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


Mewakili tipe file yang tidak diketahui.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIF() {#getTIF--}
```
public static FileType getTIF()
```


Tagged Image File (.tif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIFF() {#getTIFF--}
```
public static FileType getTIFF()
```


Tagged Image File Format (.tiff)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPG() {#getJPG--}
```
public static FileType getJPG()
```


Gambar JPEG (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


Gambar JPEG (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


Grafik Jaringan Portabel (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


Berkas Format Pertukaran Grafis (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


Berkas Gambar Bitmap (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


Berkas Gambar Inti JPEG 2000 (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


Berkas Bahasa Markah Hiperteks (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


Berkas Bahasa Markah Hiperteks (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


Berkas Format Dokumen Portabel (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


Presentasi PowerPoint (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


Presentasi PowerPoint Open XML (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


Presentasi OpenDocument (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


Templat Presentasi PowerPoint Open XML (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


Templat Presentasi PowerPoint Open XML yang Mendukung Makro (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


Templat Presentasi OpenDocument (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Lembar Kerja Excel (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Lembar Kerja Microsoft Excel Open XML (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Lembar Kerja Excel Open XML yang Mendukung Makro (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Lembar Kerja Biner Excel (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Templat Lembar Kerja Excel Open XML (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Templat Lembar Kerja Excel Open XML yang Mendukung Makro (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Templat Excel (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


Berkas Nilai Dipisahkan Koma (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


Berkas Nilai Dipisahkan Tab (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


Berkas Nilai Dipisahkan Tab (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


OpenDocument Spreadsheet (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


OpenDocument Spreadsheet Template (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Apple Numbers Spreadsheet (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


File Dokumentasi Markdown (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Microsoft Word Document (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Microsoft Word Open XML Document (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Word Open XML Macro-Enabled Document (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Word Document Template (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Word Open XML Document Template (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Word Open XML Macro-Enabled Document Template (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


File Rich Text Format (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


File Teks Biasa (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


OpenDocument Text Document (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


OpenDocument Document Template (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


Memetakan ekstensi file ke tipe file.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | ekstensi | java.lang.String | Ekstensi file (termasuk titik "."). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


Mengambil tipe file yang didukung


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - Mengembalikan urutan tipe file yang didukung

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


Menentukan apakah yang saat ini
FileType
sama dengan yang ditentukan
FileType
objek.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | Objek yang dibandingkan dengan objek  FileType  saat ini. |
|

**Returns:**
boolean - ```
true
```

if both  FileType  objects are the same; otherwise,

```
false
```


### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determines whether the current 
FileType
 is the same as specified object.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object to compare with the current  FileType  object.
 |

**Returns:**
boolean - ```
true
```

jika

```
obj
```

parameter adalah  FileType  dan sama dengan objek  FileType  saat ini; jika tidak,

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan kode hash untuk yang saat ini
FileType
objek.


**Returns:**
int - Kode hash untuk objek  FileType  saat ini.

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


Menentukan apakah dua
FileType
objek sama.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | Objek  FileType  kiri. |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | Objek  FileType  kanan. |
|

**Returns:**
boolean - ```
true
```

if both  FileType  objects are the same; otherwise,

```
false
```


### op_Inequality(FileType left, FileType right) {#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Inequality(FileType left, FileType right)
```


Determines whether two 
FileType
 objects are not the same.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| left | [FileType](../../com.groupdocs.redaction/filetype) | Left  FileType  object.
 |
| right | [FileType](../../com.groupdocs.redaction/filetype) | Right  FileType  object.
 |

**Returns:**
boolean - ```
true
```

jika kedua objek  FileType  tidak sama; jika tidak,

```
false
```


### toString() {#toString--}
```
public String toString()
```


Mengembalikan string yang merepresentasikan objek saat ini.


**Returns:**
java.lang.String - String yang mewakili objek saat ini.

