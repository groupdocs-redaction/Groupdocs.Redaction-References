---
title: "PageRangeFilter"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Bir belgede kırpma uygulamak için sayfa aralığını ayarlayan kırpma filtresini temsil eder."
type: docs
weight: 24
url: /tr/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

Redaksiyon filtresini temsil eder, bir belge içinde redaksiyon uygulanacak sayfa aralığını ayarlar.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | RemovePageRedaction sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | Belgenin başlangıcı ya da sonu olan arama referans konumunu alır. |
|
|  | [getIndex()](#getIndex--) | Başlangıç konumu indeksini alır (0 tabanlı). |
|
|  | [getCount()](#getCount--) | Kaldırılacak sayfa sayısını alır. |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | Bu filtre sayfa aralığının verilen sayfayı içerip içermediğini kontrol eder. |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


RemovePageRedaction sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | Arama referans konumu, belgenin başlangıcı ya da sonu |
|
|  | indeks | int | Başlangıç konumu indeksi (0 tabanlı) |
|
|  | sayım | int | Kaldırılacak sayfa sayısı |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


Belgenin başlangıcı ya da sonu olan arama referans konumunu alır.


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Başlangıç konumu indeksini alır (0 tabanlı).


**Returns:**
int - Başlangıç konumu indeksi (0 tabanlı).

### getCount() {#getCount--}
```
public final int getCount()
```


Kaldırılacak sayfa sayısını alır.


**Returns:**
int - Kaldırılacak sayfa sayısı.

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


Bu filtre sayfa aralığının verilen sayfayı içerip içermediğini kontrol eder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | sayfanın indeksi (sıfır tabanlı) |
|
|  | pageCount | int | toplam sayfa sayısı |
|

**Returns:**
boolean - doğru, eğer bu filtre aralığı sayfayı içeriyorsa

