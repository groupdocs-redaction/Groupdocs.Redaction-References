---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "提供された正規表現に一致させてドキュメント内のテキストを検索・置換するテキスト削除を表します。"
type: docs
weight: 28
url: /ja/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object、[com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)、[com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

提供された正規表現に一致させてドキュメント内のテキストを検索・置換するテキスト削除を表します。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | RegexRedaction クラスの新しいインスタンスを初期化します。 |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | RegexRedaction クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | 一致させる正規表現を取得します。 |
|
|  | [getDescription()](#getDescription--) | レダクションとそのパラメータを説明する文字列を返します。 |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 指定されたフォーマットインスタンスにレダクションを適用します。 |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


RegexRedaction クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pattern | java.lang.String | 検索と置換のための正規表現 |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 置換オプション（テキスト、色） |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


RegexRedaction クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | 検索と置換のための正規表現 |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 置換オプション（テキスト、色） |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


一致させる正規表現を取得します。


**Returns:**
java.util.regex.Pattern - 一致させる正規表現。

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

