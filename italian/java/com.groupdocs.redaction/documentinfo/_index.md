---
title: "DocumentInfo"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta un'informazione sul documento."
type: docs
weight: 10
url: /it/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

Rappresenta un'informazione sul documento. Implementa l'interfaccia IDocumentInfo. Vedi
IDocumentInfo
per esempi.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFileType()](#getFileType--) | Ottiene la descrizione del formato file. |
|
|  | [getPageCount()](#getPageCount--) | Ottiene il conteggio totale delle pagine. |
|
|  | [getSize()](#getSize--) | Ottiene la dimensione del documento in byte. |
|
|  | [getPages()](#getPages--) | Ottiene l'elenco delle informazioni sulla pagina. |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


Ottiene la descrizione del formato file.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Ottiene il conteggio totale delle pagine.


**Returns:**
int - Il conteggio totale delle pagine.

### getSize() {#getSize--}
```
public final long getSize()
```


Ottiene la dimensione del documento in byte.


**Returns:**
long - La dimensione del documento in byte.

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


Ottiene l'elenco delle informazioni sulla pagina.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - L'elenco delle informazioni sulla pagina.

