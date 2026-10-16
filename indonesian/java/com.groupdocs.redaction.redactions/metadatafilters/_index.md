---
title: "MetadataFilters"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili daftar tipe metadata dokumen yang paling umum."
type: docs
weight: 19
url: /id/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

Mewakili daftar tipe metadata dokumen yang paling umum.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## Bidang

| Bidang | Deskripsi |
| --- | --- |
|  | [None](#None) | Pengaturan filter kosong, tidak cocok dengan item metadata apa pun. |
|
|  | [Author](#Author) | Penulis dokumen. |
|
|  | [Category](#Category) | Kategori dokumen. |
|
|  | [Comments](#Comments) | Komentar untuk dokumen. |
|
|  | [Company](#Company) | Perusahaan Penulis. |
|
|  | [ContentStatus](#ContentStatus) | Status konten. |
|
|  | [CreatedTime](#CreatedTime) | Waktu dibuat. |
|
|  | [HyperlinkBase](#HyperlinkBase) | Basis tautan hiper. |
|
|  | [LastPrinted](#LastPrinted) | Tanggal dan waktu cetak terakhir. |
|
|  | [LastSavedBy](#LastSavedBy) | Terakhir disimpan oleh pengguna. |
|
|  | [LastSavedTime](#LastSavedTime) | Tanggal dan waktu penyimpanan terakhir. |
|
|  | [NameOfApplication](#NameOfApplication) | Nama aplikasi tempat dokumen dibuat. |
|
|  | [Manager](#Manager) | Nama manajer Penulis. |
|
|  | [RevisionNumber](#RevisionNumber) | Nomor revisi. |
|
|  | [Subject](#Subject) | Subjek dokumen. |
|
|  | [Template](#Template) | Nama templat dokumen. |
|
|  | [Title](#Title) | Judul dokumen. |
|
|  | [TotalEditingTime](#TotalEditingTime) | Total waktu penyuntingan. |
|
|  | [Version](#Version) | Versi dokumen. |
|
|  | [Description](#Description) | Deskripsi dokumen. |
|
|  | [Keywords](#Keywords) | Kata kunci dokumen. |
|
|  | [ContentType](#ContentType) | Tipe konten. |
|
|  | [All](#All) | Semua tipe item metadata. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getNames()](#getNames--) | Mendapatkan sekumpulan semua tipe filter yang dideklarasikan. |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | Mendapatkan nilai MetadataFiler berdasarkan namanya. |
|
|  | [parse(String values)](#parse-java.lang.String-) | Menganalisis string nilai MetadataFilers yang dipisahkan koma menjadi integer. |
|
|  | [toString(int value)](#toString-int-) | Menyimpan sebuah integer sebagai string nilai MetadataFilers yang dipisahkan koma. |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


Pengaturan filter kosong, tidak cocok dengan item metadata apa pun.


### Author {#Author}
```
public static final int Author
```


Penulis dokumen.


### Category {#Category}
```
public static final int Category
```


Kategori dokumen.


### Comments {#Comments}
```
public static final int Comments
```


Komentar untuk dokumen.


### Company {#Company}
```
public static final int Company
```


Perusahaan Penulis.


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


Status konten.


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


Waktu dibuat.


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


Basis tautan hiper.


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


Tanggal dan waktu cetak terakhir.


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


Terakhir disimpan oleh pengguna.


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


Tanggal dan waktu penyimpanan terakhir.


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


Nama aplikasi tempat dokumen dibuat.


### Manager {#Manager}
```
public static final int Manager
```


Nama manajer Penulis.


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


Nomor revisi.


### Subject {#Subject}
```
public static final int Subject
```


Subjek dokumen.


### Template {#Template}
```
public static final int Template
```


Nama templat dokumen.


### Title {#Title}
```
public static final int Title
```


Judul dokumen.


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


Total waktu penyuntingan.


### Version {#Version}
```
public static final int Version
```


Versi dokumen.


### Description {#Description}
```
public static final int Description
```


Deskripsi dokumen.


### Keywords {#Keywords}
```
public static final int Keywords
```


Kata kunci dokumen.


### ContentType {#ContentType}
```
public static final int ContentType
```


Tipe konten.


### All {#All}
```
public static final int All
```


Semua tipe item metadata.


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


Mendapatkan sekumpulan semua tipe filter yang dideklarasikan.


**Returns:**
java.util.Set<java.lang.String> - Sekumpulan semua tipe filter yang dideklarasikan.

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


Mendapatkan nilai MetadataFiler berdasarkan namanya.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | valueName | java.lang.String | Nama MetadataFilter. |
|

**Returns:**
int - Nilai MetadataFiler.

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


Menganalisis string nilai MetadataFilers yang dipisahkan koma menjadi integer.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | String nilai MetadataFilers yang dipisahkan koma. |
|

**Returns:**
int - Nilai MetadataFilers.

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


Menyimpan sebuah integer sebagai string nilai MetadataFilers yang dipisahkan koma.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Nilai MetadataFiler. |
|

**Returns:**
java.lang.String - String nilai MetadataFiler yang dipisahkan koma.

