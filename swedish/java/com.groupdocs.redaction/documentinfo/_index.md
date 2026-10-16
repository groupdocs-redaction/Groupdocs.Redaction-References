---
title: "DocumentInfo"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar information om ett dokument."
type: docs
weight: 10
url: /sv/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

Representerar information om dokumentet. Implementerar IDocumentInfo‑gränssnittet. Se
IDocumentInfo
för exempel.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFileType()](#getFileType--) | Hämtar filformatets beskrivning. |
|
|  | [getPageCount()](#getPageCount--) | Hämtar det totala sidantalet. |
|
|  | [getSize()](#getSize--) | Hämtar dokumentets storlek i byte. |
|
|  | [getPages()](#getPages--) | Hämtar listan med sidinformation. |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


Hämtar filformatets beskrivning.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Hämtar det totala sidantalet.


**Returns:**
int – Det totala sidantalet.

### getSize() {#getSize--}
```
public final long getSize()
```


Hämtar dokumentets storlek i byte.


**Returns:**
long – Dokumentets storlek i byte.

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


Hämtar listan med sidinformation.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> – Listan med sidinformation.

