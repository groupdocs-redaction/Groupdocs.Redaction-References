---
title: "DocumentInfo"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет информацию о документе."
type: docs
weight: 10
url: /ru/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

Представляет информацию о документе. Реализует интерфейс IDocumentInfo. См
IDocumentInfo
для примеров.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Методы

| Метод | Описание |
| --- | --- |
|  | [getFileType()](#getFileType--) | Получает описание формата файла. |
|
|  | [getPageCount()](#getPageCount--) | Получает общее количество страниц. |
|
|  | [getSize()](#getSize--) | Получает размер документа в байтах. |
|
|  | [getPages()](#getPages--) | Получает список информации о страницах. |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


Получает описание формата файла.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Получает общее количество страниц.


**Returns:**
int - Общее количество страниц.

### getSize() {#getSize--}
```
public final long getSize()
```


Получает размер документа в байтах.


**Returns:**
long - Размер документа в байтах.

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


Получает список информации о страницах.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - Список информации о страницах.

