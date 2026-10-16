---
title: "IDocumentInfo"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "기본 문서 정보를 가져오는 데 필요한 메서드를 정의합니다."
type: docs
weight: 19
url: /ko/java/com.groupdocs.redaction/idocumentinfo/
---```
public interface IDocumentInfo
```

Defines methods that are required for getting basic document information.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Methods

| Method | Description |
| --- | --- |
| [getFileType()](#getFileType--) | Gets the file format description.
 |
| [getPageCount()](#getPageCount--) | Gets the total page count.
 |
| [getSize()](#getSize--) | Gets the document size in bytes.
 |
| [getPages()](#getPages--) | Gets the list of page information.
 |
### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Gets the file format description.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


Gets the total page count.


**Returns:**
int - The total page count.

### getSize() {#getSize--}
```
public abstract long getSize()
```


Gets the document size in bytes.


**Returns:**
long - The document size in bytes.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


Gets the list of page information.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - The list of page information.

