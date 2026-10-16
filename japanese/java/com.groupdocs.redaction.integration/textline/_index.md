---
title: "TextLine"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "画像からOCRエンジンによって抽出されたテキスト行を表します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

OCR エンジンが画像から抽出したテキストの行を表します。

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | 画像からOCRエンジンによって抽出されたテキスト行の新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFragments()](#getFragments--) | 行内で認識された記号や単語などのテキストフラグメントの配列を取得します。 |
|
|  | [toString()](#toString--) | 認識されたテキスト行の文字内容を返します。 |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


画像からOCRエンジンによって抽出されたテキスト行の新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | テキストフラグメントの初期セット |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


行内で認識された記号や単語などのテキストフラグメントの配列を取得します。


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - 行で認識されたシンボルや単語などのテキストフラグメントの配列。

### toString() {#toString--}
```
public String toString()
```


認識されたテキスト行の文字内容を返します。


**Returns:**
java.lang.String - 認識されたテキスト行の文字内容

