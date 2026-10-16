---
title: "DocumentInfo"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "문서에 대한 정보를 나타냅니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

문서에 대한 정보를 나타냅니다. IDocumentInfo 인터페이스를 구현합니다. 참조
IDocumentInfo
예제에 대해.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFileType()](#getFileType--) | 파일 형식 설명을 가져옵니다. |
|
|  | [getPageCount()](#getPageCount--) | 전체 페이지 수를 가져옵니다. |
|
|  | [getSize()](#getSize--) | 문서 크기를 바이트 단위로 가져옵니다. |
|
|  | [getPages()](#getPages--) | 페이지 정보 목록을 가져옵니다. |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


파일 형식 설명을 가져옵니다.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


전체 페이지 수를 가져옵니다.


**Returns:**
int - 전체 페이지 수.

### getSize() {#getSize--}
```
public final long getSize()
```


문서 크기를 바이트 단위로 가져옵니다.


**Returns:**
long - 문서 크기(바이트).

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


페이지 정보 목록을 가져옵니다.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - 페이지 정보 목록.

