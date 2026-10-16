---
title: "RedactorLogEntry"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "編集適用の結果を表します。"
type: docs
weight: 18
url: /ja/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

編集適用の結果を表します。

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | Redaction 用に RedactorLogEntry クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getResult()](#getResult--) | 結果を取得します、返されるのは |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | リダクションへの参照とそのオプションを取得します。 |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


Redaction 用に RedactorLogEntry クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | リダクションへの参照 |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | フォーマットハンドラが報告するリダクション結果 |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


結果を取得します、返されるのは
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


リダクションへの参照とそのオプションを取得します。


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

