---
title: "CustomRedactionContext"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "入力データを提供します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) の入力データを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | 利用可能な場合、マッチしたフラグメントのページ番号を取得します。 |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | マッチしたフラグメントのページ番号を設定します。 |
|
|  | [getText()](#getText--) | リダクション用にマッチしたテキストを取得します。 |
|
|  | [setText(String value)](#setText-java.lang.String-) | リダクション用にマッチしたテキストを設定します。 |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


利用可能な場合、マッチしたフラグメントのページ番号を取得します。


**Returns:**
int - ページ番号、またはページが不明な場合のフォーマット固有の値です。

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


マッチしたフラグメントのページ番号を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | int | ページ番号です。 |
|

### getText() {#getText--}
```
public final String getText()
```


リダクション用にマッチしたテキストを取得します。


**Returns:**
java.lang.String - マッチしたテキストです。

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


リダクション用にマッチしたテキストを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | マッチしたテキストです。 |
|

