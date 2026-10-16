---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "最も一般的なドキュメントメタデータのタイプの一覧を表します。"
type: docs
weight: 19
url: /ja/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

最も一般的なドキュメントメタデータのタイプの一覧を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## フィールド

| フィールド | 説明 |
| --- | --- |
|  | [None](#None) | 空のフィルター設定で、メタデータ項目に一致しません。 |
|
|  | [Author](#Author) | 文書の作成者。 |
|
|  | [Category](#Category) | 文書のカテゴリ。 |
|
|  | [Comments](#Comments) | 文書のコメント。 |
|
|  | [Company](#Company) | 作成者の会社。 |
|
|  | [ContentStatus](#ContentStatus) | コンテンツのステータス。 |
|
|  | [CreatedTime](#CreatedTime) | 作成日時。 |
|
|  | [HyperlinkBase](#HyperlinkBase) | ハイパーリンクのベース。 |
|
|  | [LastPrinted](#LastPrinted) | 最終印刷日時。 |
|
|  | [LastSavedBy](#LastSavedBy) | ユーザーによる最終保存。 |
|
|  | [LastSavedTime](#LastSavedTime) | 最終保存日時。 |
|
|  | [NameOfApplication](#NameOfApplication) | 文書が作成されたアプリケーションの名前。 |
|
|  | [Manager](#Manager) | 作成者の上司の名前。 |
|
|  | [RevisionNumber](#RevisionNumber) | リビジョン番号。 |
|
|  | [Subject](#Subject) | 文書の件名。 |
|
|  | [Template](#Template) | 文書テンプレート名。 |
|
|  | [Title](#Title) | 文書のタイトル。 |
|
|  | [TotalEditingTime](#TotalEditingTime) | 総編集時間。 |
|
|  | [Version](#Version) | 文書のバージョン。 |
|
|  | [Description](#Description) | 文書の説明。 |
|
|  | [Keywords](#Keywords) | 文書のキーワード。 |
|
|  | [ContentType](#ContentType) | コンテンツタイプ。 |
|
|  | [All](#All) | メタデータ項目のすべてのタイプ。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getNames()](#getNames--) | 宣言されたすべてのフィルタタイプのセットを取得します。 |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | 名前でMetadataFilerの値を取得します。 |
|
|  | [parse(String values)](#parse-java.lang.String-) | カンマ区切りのMetadataFilers値の文字列をintに解析します。 |
|
|  | [toString(int value)](#toString-int-) | 整数をカンマ区切りのMetadataFilers値の文字列として保存します。 |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


空のフィルター設定で、メタデータ項目に一致しません。


### Author {#Author}
```
public static final int Author
```


文書の作成者。


### Category {#Category}
```
public static final int Category
```


文書のカテゴリ。


### Comments {#Comments}
```
public static final int Comments
```


文書のコメント。


### Company {#Company}
```
public static final int Company
```


作成者の会社。


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


コンテンツのステータス。


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


作成日時。


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


ハイパーリンクのベース。


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


最終印刷日時。


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


ユーザーによる最終保存。


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


最終保存日時。


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


文書が作成されたアプリケーションの名前。


### Manager {#Manager}
```
public static final int Manager
```


作成者の上司の名前。


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


リビジョン番号。


### Subject {#Subject}
```
public static final int Subject
```


文書の件名。


### Template {#Template}
```
public static final int Template
```


文書テンプレート名。


### Title {#Title}
```
public static final int Title
```


文書のタイトル。


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


総編集時間。


### Version {#Version}
```
public static final int Version
```


文書のバージョン。


### Description {#Description}
```
public static final int Description
```


文書の説明。


### Keywords {#Keywords}
```
public static final int Keywords
```


文書のキーワード。


### ContentType {#ContentType}
```
public static final int ContentType
```


コンテンツタイプ。


### All {#All}
```
public static final int All
```


メタデータ項目のすべてのタイプ。


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


宣言されたすべてのフィルタタイプのセットを取得します。


**Returns:**
java.util.Set<java.lang.String> - 宣言されたすべてのフィルタタイプのセット。

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


名前でMetadataFilerの値を取得します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | valueName | java.lang.String | MetadataFilterの名前。 |
|

**Returns:**
int - MetadataFilerの値。

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


カンマ区切りのMetadataFilers値の文字列をintに解析します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | values | java.lang.String | カンマ区切りのMetadataFilers値の文字列。 |
|

**Returns:**
int - MetadataFilersの値。

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


整数をカンマ区切りのMetadataFilers値の文字列として保存します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | int | MetadataFilerの値。 |
|

**Returns:**
java.lang.String - カンマ区切りのMetadataFiler値の文字列。

