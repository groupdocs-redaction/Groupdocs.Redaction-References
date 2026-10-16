---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "削除プロセス中に実行された単一の変更アクション情報を表します。"
type: docs
weight: 25
url: /ja/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

削除プロセス中に実行された単一の変更アクション情報を表します。

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | 置換情報なしで RedactionDescription クラスの新しいインスタンスを初期化します。 |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | 置換情報付きで RedactionDescription クラスの新しいインスタンスを初期化します。 |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | 画像領域の置換情報付きで RedactionDescription クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | ドキュメントデータのタイプ（テキスト、メタデータ、または注釈）を取得します。 |
|
|  | [getActionType()](#getActionType--) | 削除操作（置換、クリーンアップ、または削除）を取得します。 |
|
|  | [getOriginalText()](#getOriginalText--) | 式が提供されている場合、一致したテキストを取得します。 |
|
|  | [getReplacement()](#getReplacement--) | 置換情報を取得します。null の場合があります。 |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | 画像領域の削除に対する置換情報を取得します。テキスト削除の場合は null を返します。 |
|
|  | [getDetails()](#getDetails--) | 削除対象項目のオプションの詳細情報を取得します。 |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | 削除対象項目のオプションの詳細情報を設定します。 |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


置換情報なしで RedactionDescription クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | redactionType | int | 削除されるデータのタイプ |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | これらのデータに対して実行されるアクション |
|
|  | originalText | java.lang.String | 一致したテキスト、コメント、または注釈本文 |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


置換情報付きで RedactionDescription クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | redactionType | int | 削除されるデータのタイプ |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | これらのデータに対して実行されるアクション |
|
|  | originalText | java.lang.String | 一致したテキスト、コメント、または注釈本文 |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | 置換テキスト、一致したテキスト、および元の文字列内での位置 |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


画像領域の置換情報付きで RedactionDescription クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | redactionType | int | 削除されるデータのタイプ |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | これらのデータに対して実行されるアクション |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | 画像領域の置換情報 |
|
|  | imageDetails | java.lang.String | 画像のテキスト説明。デフォルトは String.Empty です。 |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


ドキュメントデータのタイプ（テキスト、メタデータ、または注釈）を取得します。


**Returns:**
int - ドキュメントデータのタイプ - テキスト、メタデータ、または注釈。

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


削除操作（置換、クリーンアップ、または削除）を取得します。


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


式が提供されている場合、一致したテキストを取得します。


**Returns:**
java.lang.String - 任意の式が提供された場合の一致したテキスト。

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


置換情報を取得します。null の場合があります。


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


画像領域の削除に対する置換情報を取得します。テキスト削除の場合は null を返します。


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


削除対象項目のオプションの詳細情報を取得します。


**Returns:**
java.lang.String - 赤字対象項目のオプション詳細情報。

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


削除対象項目のオプションの詳細情報を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | 赤字対象項目のオプション詳細情報。 |
|

