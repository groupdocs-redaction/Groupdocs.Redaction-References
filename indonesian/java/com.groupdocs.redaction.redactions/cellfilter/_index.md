---
title: "CellFilter"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Menyediakan opsi untuk membatasi cakupan CellColumnRedaction ke lembar kerja dan kolom."
type: docs
weight: 12
url: /id/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

Menyediakan opsi untuk membatasi ruang lingkup sebuah
CellColumnRedaction
ke lembar kerja dan kolom.

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | Menginisialisasi instance baru. |
|
## Bidang

| Bidang | Deskripsi |
| --- | --- |
|  | [NoIndex](#NoIndex) | Mewakili nilai default untuk filter, yaitu -1. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | Mendapatkan nama lembar kerja (jika berlaku). |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | Mengatur nama lembar kerja (jika berlaku). |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | Mendapatkan indeks lembar kerja (berbasis nol). |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | Mengatur indeks lembar kerja (berbasis nol). |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | Mendapatkan nilai yang menunjukkan apakah |
WorkSheetIndex
apakah diatur atau tidak.
|
|  | [getColumnIndex()](#getColumnIndex--) | Mendapatkan indeks kolom (berbasis nol). |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | Mengatur indeks kolom (berbasis nol). |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


Menginisialisasi instance baru.


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


Mewakili nilai default untuk filter, yaitu -1.


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


Mendapatkan nama lembar kerja (jika berlaku).


**Returns:**
java.lang.String - Nama lembar kerja (jika berlaku).

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


Mengatur nama lembar kerja (jika berlaku).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Nama lembar kerja (jika berlaku). |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


Mendapatkan indeks lembar kerja (berbasis nol).


**Returns:**
int - Indeks lembar kerja (berbasis nol).

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


Mengatur indeks lembar kerja (berbasis nol).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Indeks lembar kerja (berbasis nol). |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


Mendapatkan nilai yang menunjukkan apakah
WorkSheetIndex
apakah diatur atau tidak.


**Returns:**
boolean - Nilai yang menunjukkan apakah WorkSheetIndex sudah diatur atau tidak.

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


Mendapatkan indeks kolom (berbasis nol).


**Returns:**
int - Indeks kolom (berbasis nol).

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


Mengatur indeks kolom (berbasis nol).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Indeks kolom (berbasis nol). |
|

