---
title: "Redaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "すべての編集タイプの基底抽象クラスを表します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

すべての編集タイプの基底抽象クラスを表します。

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getDescription()](#getDescription--) | レダクションとそのパラメータを説明する文字列を返します。 |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 指定されたフォーマットインスタンスにレダクションを適用します。 |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


レダクションとそのパラメータを説明する文字列を返します。


**Returns:**
java.lang.String - レダクション名とパラメータを含むテキスト。

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


指定されたフォーマットインスタンスにレダクションを適用します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | レダクションを適用するドキュメントのインスタンス |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

