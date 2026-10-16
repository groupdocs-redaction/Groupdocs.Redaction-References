---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "デフォルトで大文字小文字を区別せずに、文書のテキスト内の正確なフレーズを置換するテキストの編集を表します。"
type: docs
weight: 17
url: /ja/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object、[com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)、[com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

デフォルトで大文字小文字を区別せず、ドキュメントのテキスト内の正確なフレーズを置換するテキスト赤字を表します。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

次の例は、大文字小文字を区別したフレーズ検索と置換の実行を示しています。

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
``` 
````

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

````

try (Redactor redactor = new Redactor("C:\\sample.pdf"))
{
// デフォルトでは、isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
doc.save();
}
 
``` 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | 大文字小文字を区別しないモードで ExactPhraseRedaction クラスの新しいインスタンスを初期化します。 |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | ExactPhraseRedaction クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | 検索および置換対象の文字列を取得します。 |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | 検索が大文字小文字を区別するかどうかを示す値を取得します。 |
|
|  | [isRightToLeft()](#isRightToLeft--) | このテキストが右から左へ表示されるかどうかを示す値を取得します（デフォルトは false）。 |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | このテキストが右から左へ表示されるかどうかを示す値を設定します（デフォルトは false）。 |
|
|  | [getDescription()](#getDescription--) | レダクションとそのパラメータを説明する文字列を返します。 |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 指定されたフォーマットインスタンスにレダクションを適用します。 |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


大文字小文字を区別しないモードで ExactPhraseRedaction クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | 検索および置換対象の文字列 |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 置換オプション（テキスト、色） |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


ExactPhraseRedaction クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | 検索および置換対象の文字列 |
|
|  | isCaseSensitive | boolean | 大文字小文字を区別した検索が必要な場合は true |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 置換オプション（テキスト、色） |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


検索および置換対象の文字列を取得します。


**Returns:**
java.lang.String - 検索および置換対象の文字列です。

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


検索が大文字小文字を区別するかどうかを示す値を取得します。


**Returns:**
boolean - 検索が大文字小文字を区別するかどうかを示す値です。

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


このテキストが右から左へ表示されるかどうかを示す値を取得します（デフォルトは false）。


**Returns:**
boolean - このテキストが右から左へ表示されるかどうかを示す値です（デフォルトは false）。

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


このテキストが右から左へ表示されるかどうかを示す値を設定します（デフォルトは false）。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | boolean | このテキストが右から左へ表示されるかどうかを示す値です（デフォルトは false）。 |
|

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

