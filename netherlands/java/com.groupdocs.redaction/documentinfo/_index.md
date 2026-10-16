---
title: "DocumentInfo"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt informatie over een document voor."
type: docs
weight: 10
url: /nl/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

Stelt informatie over een document voor. Implementeert de IDocumentInfo interface. Zie
IDocumentInfo
voor voorbeelden.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFileType()](#getFileType--) | Haalt de beschrijving van het bestandsformaat op. |
|
|  | [getPageCount()](#getPageCount--) | Haalt het totale aantal pagina's op. |
|
|  | [getSize()](#getSize--) | Haalt de documentgrootte in bytes op. |
|
|  | [getPages()](#getPages--) | Haalt de lijst met paginainformatie op. |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


Haalt de beschrijving van het bestandsformaat op.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Haalt het totale aantal pagina's op.


**Returns:**
int - Het totale aantal pagina's.

### getSize() {#getSize--}
```
public final long getSize()
```


Haalt de documentgrootte in bytes op.


**Returns:**
long - De documentgrootte in bytes.

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


Haalt de lijst met paginainformatie op.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - De lijst met paginainformatie.

