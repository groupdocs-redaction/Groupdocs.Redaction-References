---
title: "CellFilter"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "CellColumnRedaction kapsamını bir çalışma sayfası ve bir sütunla sınırlama seçeneği sunar."
type: docs
weight: 12
url: /tr/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

Bir şeyin kapsamını sınırlamak için bir seçenek sağlar.
CellColumnRedaction
bir çalışma sayfasına ve bir sütuna.

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | Yeni bir örnek başlatır. |
|
## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [NoIndex](#NoIndex) | Filtre için varsayılan değeri temsil eder; bu değer -1'dir. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | Bir çalışma sayfası adını alır (uygunsa). |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | Bir çalışma sayfası adını ayarlar (uygunsa). |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | Bir çalışma sayfası indeksini alır (sıfır tabanlı). |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | Bir çalışma sayfası indeksini ayarlar (sıfır tabanlı). |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | Belirtilen durumun olup olmadığını gösteren bir değeri alır |
WorkSheetIndex
ayarlanıp ayarlanmadığını.
|
|  | [getColumnIndex()](#getColumnIndex--) | Bir sütun indeksini alır (sıfır tabanlı). |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | Bir sütun indeksini ayarlar (sıfır tabanlı). |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


Yeni bir örnek başlatır.


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


Filtre için varsayılan değeri temsil eder; bu değer -1'dir.


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


Bir çalışma sayfası adını alır (uygunsa).


**Returns:**
java.lang.String - Bir çalışma sayfası adı (uygunsa).

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


Bir çalışma sayfası adını ayarlar (uygunsa).


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Bir çalışma sayfası adı (uygunsa). |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


Bir çalışma sayfası indeksini alır (sıfır tabanlı).


**Returns:**
int - Bir çalışma sayfası indeksi (sıfır tabanlı).

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


Bir çalışma sayfası indeksini ayarlar (sıfır tabanlı).


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Bir çalışma sayfası indeksi (sıfır tabanlı). |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


Belirtilen durumun olup olmadığını gösteren bir değeri alır
WorkSheetIndex
ayarlanıp ayarlanmadığını.


**Returns:**
boolean - WorkSheetIndex'in ayarlanıp ayarlanmadığını gösteren bir değer.

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


Bir sütun indeksini alır (sıfır tabanlı).


**Returns:**
int - Bir sütun indeksi (sıfır tabanlı).

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


Bir sütun indeksini ayarlar (sıfır tabanlı).


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Bir sütun indeksi (sıfır tabanlı). |
|

