---
title: "DocumentInfo"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa información sobre el documento."
type: docs
weight: 10
url: /es/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

Representa información sobre el documento. Implementa la interfaz IDocumentInfo. Ver
IDocumentInfo
para ejemplos.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFileType()](#getFileType--) | Obtiene la descripción del formato de archivo. |
|
|  | [getPageCount()](#getPageCount--) | Obtiene el recuento total de páginas. |
|
|  | [getSize()](#getSize--) | Obtiene el tamaño del documento en bytes. |
|
|  | [getPages()](#getPages--) | Obtiene la lista de información de páginas. |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


Obtiene la descripción del formato de archivo.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Obtiene el recuento total de páginas.


**Returns:**
int - El recuento total de páginas.

### getSize() {#getSize--}
```
public final long getSize()
```


Obtiene el tamaño del documento en bytes.


**Returns:**
long - El tamaño del documento en bytes.

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


Obtiene la lista de información de páginas.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - La lista de información de páginas.

