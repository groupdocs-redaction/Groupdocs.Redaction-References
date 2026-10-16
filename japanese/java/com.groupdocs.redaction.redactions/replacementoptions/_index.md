---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "一致したテキスト置換のオプションを表します。"
type: docs
weight: 31
url: /ja/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

一致したテキスト置換のオプションを表します。

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | 置換テキストをオプションとして、ReplacementOptions クラスの新しいインスタンスを初期化します。 |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | カラー矩形をオプションとして、ReplacementOptions クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getActionType()](#getActionType--) | 置換アクションを取得します：ボックスを描画またはテキストを置換。 |
|
|  | [getReplacement()](#getReplacement--) | テキスト置換値を取得します。 |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | テキスト置換値を設定します。 |
|
|  | [getBoxColor()](#getBoxColor--) | カラーを取得します |
ReplacementType.DrawBox
オプション（それ以外は無視されます）。
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | カラーを設定します |
ReplacementType.DrawBox
オプション（それ以外は無視されます）。
|
|  | [getFilters()](#getFilters--) | この赤字に適用するフィルターの配列を取得します。 |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | この赤字に適用するフィルターの配列を設定します。 |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | カスタム赤字ハンドラを取得します。 |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | カスタム赤字ハンドラを設定します。 |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


置換テキストをオプションとして、ReplacementOptions クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 置換 | java.lang.String | テキスト置換 |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


カラー矩形をオプションとして、ReplacementOptions クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | カラー | java.awt.Color | 矩形カラー |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


置換アクションを取得します：ボックスを描画またはテキストを置換。


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


テキスト置換値を取得します。


**Returns:**
java.lang.String - テキスト置換値。

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


テキスト置換値を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | テキスト置換値。 |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


カラーを取得します
ReplacementType.DrawBox
オプション（それ以外は無視されます）。


**Returns:**
java.awt.Color - ReplacementType.DrawBox オプション用のカラー（それ以外は無視されます）。

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


カラーを設定します
ReplacementType.DrawBox
オプション（それ以外は無視されます）。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.awt.Color | ReplacementType.DrawBox オプションの色（それ以外は無視されます）。 |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


この赤字に適用するフィルターの配列を取得します。


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - このレダクションで適用するフィルタの配列。

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


この赤字に適用するフィルターの配列を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | このレダクションで適用するフィルタの配列。 |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


カスタムレダクションハンドラを取得します。PDF のみ、[PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction) がサポートされています。


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


カスタムレダクションハンドラを設定します。PDF のみ、[PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction) がサポートされています。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) のインスタンス。 |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
