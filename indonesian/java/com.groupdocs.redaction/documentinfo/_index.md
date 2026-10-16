---
title: "DocumentInfo"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili informasi tentang dokumen."
type: docs
weight: 10
url: /id/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

Mewakili informasi tentang dokumen. Mengimplementasikan antarmuka IDocumentInfo. Lihat
IDocumentInfo
untuk contoh.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFileType()](#getFileType--) | Mendapatkan deskripsi format file. |
|
|  | [getPageCount()](#getPageCount--) | Mendapatkan total jumlah halaman. |
|
|  | [getSize()](#getSize--) | Mendapatkan ukuran dokumen dalam byte. |
|
|  | [getPages()](#getPages--) | Mendapatkan daftar informasi halaman. |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


Mendapatkan deskripsi format file.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Mendapatkan total jumlah halaman.


**Returns:**
int - Total jumlah halaman.

### getSize() {#getSize--}
```
public final long getSize()
```


Mendapatkan ukuran dokumen dalam byte.


**Returns:**
long - Ukuran dokumen dalam byte.

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


Mendapatkan daftar informasi halaman.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - Daftar informasi halaman.

