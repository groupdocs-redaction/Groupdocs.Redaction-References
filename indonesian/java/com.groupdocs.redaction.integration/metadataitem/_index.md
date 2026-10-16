---
title: "MetadataItem"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili sebuah item metadata yang umum untuk semua format yang didukung dan digunakan dalam redaksi metadata."
type: docs
weight: 12
url: /id/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Mewakili item metadata, umum untuk semua format yang didukung dan digunakan dalam redaksi metadata.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | Menginisialisasi instance baru. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | Mendapatkan nama asli dari item metadata, sebagaimana muncul dalam dokumen. |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | Mengatur nama asli dari item metadata, sebagaimana muncul dalam dokumen. |
|
|  | [getCategory()](#getCategory--) | Mendapatkan kategori dari item metadata, misalnya ID sumber daya untuk item metadata sumber daya yang disematkan. |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | Mengatur kategori item metadata, misalnya ID sumber daya untuk item metadata sumber daya yang disematkan. |
|
|  | [getFilter()](#getFilter--) | Mendapatkan nilai dari |
MetadataFilters
, yang ditetapkan pada item metadata ini yang digunakan dalam filtrasi item.
|
|  | [setFilter(int value)](#setFilter-int-) | Mengatur nilai dari |
MetadataFilters
, yang ditetapkan pada item metadata ini yang digunakan dalam filtrasi item.
|
|  | [getValues()](#getValues--) | Mendapatkan nilai item metadata. |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | Mengatur nilai item metadata. |
|
|  | [isCustom()](#isCustom--) | Mendapatkan nilai yang menunjukkan apakah item ini bersifat khusus (ditambahkan oleh penulis dokumen). |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | Mengatur nilai yang menunjukkan apakah item ini bersifat khusus (ditambahkan oleh penulis dokumen). |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | Mendapatkan kunci kamus untuk , menggunakan OriginalName dan data lainnya. |
|
|  | [createClone()](#createClone--) | Membuat klon mendalam dari instance saat ini. |
|
|  | [getActualValue()](#getActualValue--) | Mendapatkan representasi string dari nilai item metadata. |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


Menginisialisasi instance baru.


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


Mendapatkan nama asli dari item metadata, sebagaimana muncul dalam dokumen.


**Returns:**
java.lang.String - Nama asli item metadata, sebagaimana muncul dalam dokumen.

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


Mengatur nama asli dari item metadata, sebagaimana muncul dalam dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Nama asli item metadata, sebagaimana muncul dalam dokumen. |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


Mendapatkan kategori dari item metadata, misalnya ID sumber daya untuk item metadata sumber daya yang disematkan.


**Returns:**
java.lang.String - Kategori item metadata, misalnya ID sumber daya untuk item metadata sumber daya yang disematkan.

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Mengatur kategori item metadata, misalnya ID sumber daya untuk item metadata sumber daya yang disematkan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Kategori item metadata, misalnya ID sumber daya untuk item metadata sumber daya yang disematkan. |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


Mendapatkan nilai dari
MetadataFilters
, yang ditetapkan pada item metadata ini yang digunakan dalam filtrasi item.


**Returns:**
int - Nilai dari  MetadataFilters , yang ditetapkan pada item metadata ini yang digunakan dalam filtrasi item.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Mengatur nilai dari
MetadataFilters
, yang ditetapkan pada item metadata ini yang digunakan dalam filtrasi item.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Nilai dari  MetadataFilters , yang ditetapkan pada item metadata ini yang digunakan dalam filtrasi item. |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


Mendapatkan nilai item metadata.


**Returns:**
java.util.List<java.lang.String> - Nilai item metadata.

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


Mengatur nilai item metadata.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.util.List<java.lang.String> | Nilai item metadata. |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


Mendapatkan nilai yang menunjukkan apakah item ini bersifat khusus (ditambahkan oleh penulis dokumen).


**Returns:**
boolean - Nilai yang menunjukkan apakah item ini bersifat khusus (ditambahkan oleh penulis dokumen).

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


Mengatur nilai yang menunjukkan apakah item ini bersifat khusus (ditambahkan oleh penulis dokumen).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah item ini bersifat khusus (ditambahkan oleh penulis dokumen). |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


Mendapatkan kunci kamus untuk , menggunakan OriginalName dan data lainnya.


**Returns:**
java.lang.String - Kunci kamus untuk , menggunakan OriginalName dan data lainnya.

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


Membuat klon mendalam dari instance saat ini.


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


Mendapatkan representasi string dari nilai item metadata.


**Returns:**
java.lang.String - Representasi string dari nilai item metadata.

