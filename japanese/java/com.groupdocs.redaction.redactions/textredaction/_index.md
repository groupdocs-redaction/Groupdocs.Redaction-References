---
title: "TextRedaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "ドキュメントテキスト削除のための基本抽象クラスを表します。"
type: docs
weight: 32
url: /ja/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

ドキュメントテキスト削除のための基本抽象クラスを表します。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | 取得します |
ReplacementOptions
インスタンス、テキスト置換のタイプを指定します。
|
|  | [getOcrConnector()](#getOcrConnector--) | 取得します |
IOcrConnector
実装、グラフィック コンテンツからテキストを抽出するために必要です。
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | 設定します |
IOcrConnector
実装、グラフィック コンテンツからテキストを抽出するために必要です。
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


取得します
ReplacementOptions
インスタンス、テキスト置換のタイプを指定します。


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


取得します
IOcrConnector
実装、グラフィック コンテンツからテキストを抽出するために必要です。


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


設定します
IOcrConnector
実装、グラフィック コンテンツからテキストを抽出するために必要です。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector の実装で、グラフィック コンテンツからテキストを抽出するために必要です。 |
|

