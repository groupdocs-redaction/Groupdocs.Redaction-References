---
title: DocumentInfo
second_title: GroupDocs.Redaction for Java API Reference
description: Represents an information about document.
type: docs
weight: 10
url: /java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

Represents an information about document. Implements IDocumentInfo interface. See  IDocumentInfo  for examples.

--------------------

**Learn more**

 *  [Get file info][]


[Get file info]: https://docs.groupdocs.com/redaction/java/get-file-info/
## Methods

| Method | Description |
| --- | --- |
| [getFileType()](#getFileType--) | Gets the file format description. |
| [getPageCount()](#getPageCount--) | Gets the total page count. |
| [getSize()](#getSize--) | Gets the document size in bytes. |
| [getPages()](#getPages--) | Gets the list of page information. |
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


Gets the file format description.

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Gets the total page count.

**Returns:**
int - The total page count.
### getSize() {#getSize--}
```
public final long getSize()
```


Gets the document size in bytes.

**Returns:**
long - The document size in bytes.
### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


Gets the list of page information.

**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - The list of page information.
