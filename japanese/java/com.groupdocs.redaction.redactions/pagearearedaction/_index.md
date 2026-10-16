---
title: "PageAreaRedaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "ページの領域内のテキスト画像および注釈に影響を与える複雑なテキスト削除を表します。"
type: docs
weight: 23
url: /ja/java/com.groupdocs.redaction.redactions/pagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction), [com.groupdocs.redaction.redactions.RegexRedaction](../../com.groupdocs.redaction.redactions/regexredaction)
```
public class PageAreaRedaction extends RegexRedaction
```

ページの領域内のテキスト、画像、注釈に影響を与える複合的なテキスト削除を表します。

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](../https://docs.groupdocs.com/redaction/java/use-page-area-redaction/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | PageAreaRedaction クラスの新しいインスタンスを初期化します。 |
|
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | PageAreaRedaction クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getImageOptions()](#getImageOptions--) | 取得します |
RegionReplacementOptions
色と領域パラメータを持つオプション。
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 指定されたフォーマットインスタンスにレダクションを適用します。 |
|
### PageAreaRedaction(Pattern regex, ReplacementOptions options) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options)
```


PageAreaRedaction クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | 検索と置換のための正規表現 |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 置換オプション（テキスト、色） |
|

### PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)
```


PageAreaRedaction クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | 検索と置換のための正規表現 |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 置換オプション（テキスト、色） |
|
|  | imageOptions | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | 置換オプション（画像領域） |
|

### getImageOptions() {#getImageOptions--}
```
public final RegionReplacementOptions getImageOptions()
```


取得します
RegionReplacementOptions
色と領域パラメータを持つオプション。


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

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

