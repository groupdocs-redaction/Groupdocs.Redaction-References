---
title: "DocumentInfo"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente une information sur le document."
type: docs
weight: 10
url: /fr/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

Représente une information sur le document. Implémente l'interface IDocumentInfo. Voir
IDocumentInfo
pour des exemples.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getFileType()](#getFileType--) | Obtient la description du format de fichier. |
|
|  | [getPageCount()](#getPageCount--) | Obtient le nombre total de pages. |
|
|  | [getSize()](#getSize--) | Obtient la taille du document en octets. |
|
|  | [getPages()](#getPages--) | Obtient la liste des informations de page. |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


Obtient la description du format de fichier.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Obtient le nombre total de pages.


**Returns:**
int - Le nombre total de pages.

### getSize() {#getSize--}
```
public final long getSize()
```


Obtient la taille du document en octets.


**Returns:**
long - La taille du document en octets.

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


Obtient la liste des informations de page.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - La liste des informations de page.

