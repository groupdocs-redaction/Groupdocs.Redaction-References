---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "画像ドキュメントの指定領域にカラー矩形を配置する赤字を表します。"
type: docs
weight: 18
url: /ja/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

画像ドキュメントの指定領域にカラー矩形を配置する赤字を表します。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | 特定の領域サイズをリダクトするための ImageAreaRedaction クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getOptions()](#getOptions--) | 取得します |
RegionReplacementOptions
色と領域パラメータを持つオプション。
|
|  | [getTopLeft()](#getTopLeft--) | 削除する領域の左上位置を取得します |
|
|  | [getDescription()](#getDescription--) | レダクションとそのパラメータを説明する文字列を返します。 |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 指定されたフォーマットインスタンスにレダクションを適用します。 |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


特定の領域サイズをリダクトするための ImageAreaRedaction クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | topLeft | java.awt.Point | 左上領域の座標 |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | 領域のサイズと色 |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


取得します
RegionReplacementOptions
色と領域パラメータを持つオプション。


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


削除する領域の左上位置を取得します


**Returns:**
java.awt.Point - 削除する領域の左上位置です

### getDescription() {#getDescription--}
```
public String getDescription()
```


レダクションとそのパラメータを説明する文字列を返します。


**Returns:**
java.lang.String - レダクション名とパラメータを含むテキスト。

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


指定されたフォーマットインスタンスにレダクションを適用します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | レダクションを適用するドキュメントのインスタンス |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

