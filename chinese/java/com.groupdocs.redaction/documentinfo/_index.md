---
title: "DocumentInfo"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示有关文档的信息。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

表示文档的信息。实现 IDocumentInfo 接口。参见
IDocumentInfo
示例。

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFileType()](#getFileType--) | 获取文件格式描述。 |
|
|  | [getPageCount()](#getPageCount--) | 获取总页数。 |
|
|  | [getSize()](#getSize--) | 获取文档大小（字节）。 |
|
|  | [getPages()](#getPages--) | 获取页面信息列表。 |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


获取文件格式描述。


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


获取总页数。


**Returns:**
int - 总页数。

### getSize() {#getSize--}
```
public final long getSize()
```


获取文档大小（字节）。


**Returns:**
long - 文档大小（字节）。

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


获取页面信息列表。


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - 页面信息列表。

