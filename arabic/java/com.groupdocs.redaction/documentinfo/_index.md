---
title: "DocumentInfo"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل معلومات عن المستند."
type: docs
weight: 10
url: /ar/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

يمثل معلومات حول المستند. ينفذ واجهة IDocumentInfo. انظر
IDocumentInfo
لأمثلة.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getFileType()](#getFileType--) | يحصل على وصف تنسيق الملف. |
|
|  | [getPageCount()](#getPageCount--) | يحصل على إجمالي عدد الصفحات. |
|
|  | [getSize()](#getSize--) | يحصل على حجم المستند بالبايت. |
|
|  | [getPages()](#getPages--) | يحصل على قائمة معلومات الصفحات. |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


يحصل على وصف تنسيق الملف.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


يحصل على إجمالي عدد الصفحات.


**Returns:**
int - إجمالي عدد الصفحات.

### getSize() {#getSize--}
```
public final long getSize()
```


يحصل على حجم المستند بالبايت.


**Returns:**
long - حجم المستند بالبايت.

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


يحصل على قائمة معلومات الصفحات.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - قائمة معلومات الصفحات.

