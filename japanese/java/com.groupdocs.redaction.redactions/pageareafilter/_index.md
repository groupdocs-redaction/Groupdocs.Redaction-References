---
title: "PageAreaFilter"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "ドキュメントのページ内の領域に削除処理を適用するための削除フィルタを表します。"
type: docs
weight: 22
url: /ja/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

ドキュメントのページ内の領域を設定して削除を適用する削除フィルターを表します。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | 特定の領域を削除するために PageAreaFilter クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | ページ上の矩形（領域の左上位置とサイズ）を取得します。 |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | このフィルタ領域が指定された矩形と交差しているかどうかをチェックします。 |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


特定の領域を削除するために PageAreaFilter クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | topLeft | java.awt.Point | 左上領域の座標 |
|
|  | サイズ | java.awt.Dimension | 領域のサイズと色 |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


ページ上の矩形（領域の左上位置とサイズ）を取得します。


**Returns:**
java.awt.Rectangle - ページ上の矩形（領域の左上位置とサイズ）

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


このフィルタ領域が指定された矩形と交差しているかどうかをチェックします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 矩形 | java.awt.Rectangle | チェック対象の矩形 |
|

**Returns:**
boolean - true、フィルター領域に交差がある場合

