---
title: "TextFragment"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "OCRエンジンによって抽出された認識テキスト（単語、記号など）の一部を表します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

OCR エンジンによって抽出された、認識されたテキスト（単語、記号など）の一部を表します。

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | 認識されたテキストフラグメントの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getText()](#getText--) | 認識されたテキストフラグメントのテキスト内容を取得します。 |
|
|  | [getRectangle()](#getRectangle--) | 認識されたテキストフラグメントのバウンディング矩形を取得します。 |
|
|  | [toString()](#toString--) | 認識されたテキストフラグメントのテキスト内容を返します。 |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


認識されたテキストフラグメントの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | text | java.lang.String | 認識されたテキストフラグメントのテキスト内容 |
|
|  | 矩形 | java.awt.Rectangle | 認識されたテキストフラグメントのバウンディング矩形 |
|

### getText() {#getText--}
```
public final String getText()
```


認識されたテキストフラグメントのテキスト内容を取得します。


**Returns:**
java.lang.String - 認識されたテキストフラグメントのテキスト内容です。

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


認識されたテキストフラグメントのバウンディング矩形を取得します。


**Returns:**
java.awt.Rectangle - 認識されたテキストフラグメントのバウンディング矩形です。

### toString() {#toString--}
```
public String toString()
```


認識されたテキストフラグメントのテキスト内容を返します。


**Returns:**
java.lang.String - 認識されたテキストフラグメントのテキスト内容

