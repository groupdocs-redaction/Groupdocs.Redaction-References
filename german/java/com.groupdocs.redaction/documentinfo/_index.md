---
title: "DocumentInfo"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Informationen über ein Dokument dar."
type: docs
weight: 10
url: /de/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

Stellt Informationen über ein Dokument dar. Implementiert das IDocumentInfo-Interface. Siehe
IDocumentInfo
für Beispiele.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFileType()](#getFileType--) | Liefert die Dateiformatbeschreibung. |
|
|  | [getPageCount()](#getPageCount--) | Liefert die Gesamtseitenzahl. |
|
|  | [getSize()](#getSize--) | Liefert die Dokumentgröße in Bytes. |
|
|  | [getPages()](#getPages--) | Liefert die Liste der Seiteninformationen. |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


Liefert die Dateiformatbeschreibung.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Liefert die Gesamtseitenzahl.


**Returns:**
int - Die Gesamtseitenzahl.

### getSize() {#getSize--}
```
public final long getSize()
```


Liefert die Dokumentgröße in Bytes.


**Returns:**
long - Die Dokumentgröße in Bytes.

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


Liefert die Liste der Seiteninformationen.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - Die Liste der Seiteninformationen.

