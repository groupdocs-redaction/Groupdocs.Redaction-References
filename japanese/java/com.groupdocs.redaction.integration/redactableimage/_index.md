---
title: "RedactableImage"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "すべてのラスター画像編集操作へのファサードを提供します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

すべてのラスター画像編集操作へのファサードを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | オブジェクトを使用して新しいインスタンスを作成し、実装します |
IImageFormatInstance
インターフェイス。
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | オブジェクトを使用して新しいインスタンスを作成し、実装します |
IMultipleAreaRedactable
インターフェイス。
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | 実際の画像コンテンツを含むストリームを取得します。 |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | 同じ色で複数の画像領域を一度に赤塗りします。 |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | 指定されたポイントの領域を、特定の色とサイズの矩形で置き換えます。 |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


オブジェクトを使用して新しいインスタンスを作成し、実装します
IImageFormatInstance
インターフェイス。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | IImageFormatInstance インターフェイスを実装したインスタンス |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


オブジェクトを使用して新しいインスタンスを作成し、実装します
IMultipleAreaRedactable
インターフェイス。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | IMultipleAreaRedactable インターフェイスを実装したインスタンス |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


実際の画像コンテンツを含むストリームを取得します。


**Returns:**
java.io.InputStream - 画像データを含むストリーム

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


同じ色で複数の画像領域を一度に赤塗りします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 矩形 | java.awt.Rectangle[] | 矩形領域の配列 |
|
|  | boxColor | java.awt.Color | 領域を塗りつぶす色 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


指定されたポイントの領域を、特定の色とサイズの矩形で置き換えます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | topLeft | java.awt.Point | 塗りつぶされた領域の左上隅の座標 |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | 色とサイズの設定 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

