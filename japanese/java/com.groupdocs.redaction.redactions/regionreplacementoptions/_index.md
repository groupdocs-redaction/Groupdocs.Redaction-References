---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "画像領域置換のための色と領域パラメータを表します。"
type: docs
weight: 29
url: /ja/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

画像領域置換のための色と領域パラメータを表します。参照
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | RegionReplacementOptions クラスの新しいインスタンスを初期化します。 |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | RegionReplacementOptions クラスの新しいインスタンスを初期化します（サイズが指定されたテキストに一致します）。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | 編集された領域を塗りつぶす色を取得します。 |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | 編集された領域を塗りつぶす色を設定します。 |
|
|  | [getSize()](#getSize--) | 幅と高さを持つ矩形を取得します。 |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | 幅と高さを持つ矩形を設定します。 |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


RegionReplacementOptions クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | fillColor | java.awt.Color | 領域を塗りつぶす色 |
|
|  | サイズ | java.awt.Dimension | 塗りつぶされた領域のサイズ |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


RegionReplacementOptions クラスの新しいインスタンスを初期化します（サイズが指定されたテキストに一致します）。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | fillColor | java.awt.Color | 領域を塗りつぶす色 |
|
|  | font | java.awt.Font | 期待されるテキストフォント |
|
|  | expectedText | java.lang.String | 期待されるテキスト |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


編集された領域を塗りつぶす色を取得します。


**Returns:**
java.awt.Color - 編集された領域を塗りつぶす色。

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


編集された領域を塗りつぶす色を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.awt.Color | 編集された領域を塗りつぶす色。 |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


幅と高さを持つ矩形を取得します。


**Returns:**
java.awt.Dimension - 幅と高さを持つ矩形。

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


幅と高さを持つ矩形を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.awt.Dimension | 幅と高さを持つ矩形。 |
|

