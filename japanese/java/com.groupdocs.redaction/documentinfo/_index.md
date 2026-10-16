---
title: "DocumentInfo"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "ドキュメントに関する情報を表します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

ドキュメントに関する情報を表します。IDocumentInfo インターフェイスを実装します。参照してください
IDocumentInfo
例について。

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFileType()](#getFileType--) | ファイル形式の説明を取得します。 |
|
|  | [getPageCount()](#getPageCount--) | 総ページ数を取得します。 |
|
|  | [getSize()](#getSize--) | ドキュメントのサイズ（バイト）を取得します。 |
|
|  | [getPages()](#getPages--) | ページ情報のリストを取得します。 |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


ファイル形式の説明を取得します。


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


総ページ数を取得します。


**Returns:**
int - 総ページ数。

### getSize() {#getSize--}
```
public final long getSize()
```


ドキュメントのサイズ（バイト）を取得します。


**Returns:**
long - ドキュメントのサイズ（バイト）。

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


ページ情報のリストを取得します。


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - ページ情報のリスト。

