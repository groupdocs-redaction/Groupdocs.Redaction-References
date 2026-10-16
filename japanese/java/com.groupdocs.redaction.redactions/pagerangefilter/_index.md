---
title: "PageRangeFilter"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "文書内で赤字処理を適用するためのページ範囲設定フィルタを表します。"
type: docs
weight: 24
url: /ja/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

ドキュメント内のページ範囲を設定して削除を適用する削除フィルターを表します。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | RemovePageRedaction クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | ドキュメントの先頭または末尾のシーク参照位置を取得します。 |
|
|  | [getIndex()](#getIndex--) | 開始位置インデックス (0ベース) を取得します。 |
|
|  | [getCount()](#getCount--) | 削除するページ数を取得します。 |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | このフィルタのページ範囲が指定されたページを含むかどうかを確認します。 |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


RemovePageRedaction クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | ドキュメントの先頭または末尾のシーク参照位置 |
|
|  | インデックス | int | 開始位置インデックス (0ベース) |
|
|  | カウント | int | 削除するページの数 |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


ドキュメントの先頭または末尾のシーク参照位置を取得します。


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


開始位置インデックス (0ベース) を取得します。


**Returns:**
int - 開始位置インデックス (0ベース)。

### getCount() {#getCount--}
```
public final int getCount()
```


削除するページ数を取得します。


**Returns:**
int - 削除するページの数。

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


このフィルタのページ範囲が指定されたページを含むかどうかを確認します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ページのインデックス (0ベース) |
|
|  | pageCount | int | 総ページ数 |
|

**Returns:**
boolean - このフィルタ範囲がページを含む場合は true

