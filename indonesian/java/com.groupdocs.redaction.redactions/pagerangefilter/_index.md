---
title: "PageRangeFilter"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili filter redaksi yang mengatur rentang halaman dalam dokumen untuk menerapkan redaksi."
type: docs
weight: 24
url: /id/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

Mewakili filter redaksi, mengatur rentang halaman dalam dokumen untuk menerapkan redaksi.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | Menginisialisasi instansi baru dari kelas RemovePageRedaction. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | Mendapatkan posisi referensi pencarian, awal atau akhir dokumen. |
|
|  | [getIndex()](#getIndex--) | Mendapatkan indeks posisi mulai (berbasis 0). |
|
|  | [getCount()](#getCount--) | Mendapatkan jumlah halaman yang akan dihapus. |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | Memeriksa apakah rentang halaman filter ini berisi halaman yang diberikan. |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


Menginisialisasi instansi baru dari kelas RemovePageRedaction.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | Posisi referensi pencarian, awal atau akhir dokumen. |
|
|  | indeks | int | Indeks posisi mulai (berbasis 0) |
|
|  | jumlah | int | Jumlah halaman yang akan dihapus |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


Mendapatkan posisi referensi pencarian, awal atau akhir dokumen.


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Mendapatkan indeks posisi mulai (berbasis 0).


**Returns:**
int - Indeks posisi mulai (berbasis nol).

### getCount() {#getCount--}
```
public final int getCount()
```


Mendapatkan jumlah halaman yang akan dihapus.


**Returns:**
int - Jumlah halaman yang akan dihapus.

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


Memeriksa apakah rentang halaman filter ini berisi halaman yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | indeks halaman (berbasis nol) |
|
|  | pageCount | int | total jumlah halaman |
|

**Returns:**
boolean - true, jika rentang filter ini berisi halaman

