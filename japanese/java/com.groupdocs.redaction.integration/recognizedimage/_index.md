---
title: "RecognizedImage"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "画像から抽出されたテキストを、認識プロセスの結果として表します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

画像から認識プロセスの結果として抽出されたテキストを表します。

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | 認識された行のセットを使用して、クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getText()](#getText--) | 構造化テキストのテキスト表現を取得します。 |
|
|  | [getLines()](#getLines--) | ドキュメント内で認識されたテキスト行とそのフラグメントを取得します。 |
|
|  | [toString()](#toString--) | 構造化テキストのテキスト表現を取得します。 |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


認識された行のセットを使用して、クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | 認識された行の IEnumerable（例：リストまたは配列） |
|

### getText() {#getText--}
```
public final String getText()
```


構造化テキストのテキスト表現を取得します。


**Returns:**
java.lang.String - 構造化テキストのテキスト表現。

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


ドキュメント内で認識されたテキスト行とそのフラグメントを取得します。


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - ドキュメント内で認識されたテキスト行とそのフラグメント。

### toString() {#toString--}
```
public String toString()
```


構造化テキストのテキスト表現を取得します。


**Returns:**
java.lang.String - 認識されたテキスト

