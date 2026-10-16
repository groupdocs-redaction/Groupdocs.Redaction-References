---
title: "DocumentInfo"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Belge hakkında bir bilgi temsil eder."
type: docs
weight: 10
url: /tr/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

Belge hakkında bilgi temsil eder. IDocumentInfo arayüzünü uygular. Bakınız
IDocumentInfo
örnekler için.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFileType()](#getFileType--) | Dosya formatı açıklamasını alır. |
|
|  | [getPageCount()](#getPageCount--) | Toplam sayfa sayısını alır. |
|
|  | [getSize()](#getSize--) | Belgenin bayt cinsinden boyutunu alır. |
|
|  | [getPages()](#getPages--) | Sayfa bilgileri listesini alır. |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


Dosya formatı açıklamasını alır.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Toplam sayfa sayısını alır.


**Returns:**
int - Toplam sayfa sayısı.

### getSize() {#getSize--}
```
public final long getSize()
```


Belgenin bayt cinsinden boyutunu alır.


**Returns:**
long - Belgenin bayt cinsinden boyutu.

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


Sayfa bilgileri listesini alır.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - Sayfa bilgileri listesi.

