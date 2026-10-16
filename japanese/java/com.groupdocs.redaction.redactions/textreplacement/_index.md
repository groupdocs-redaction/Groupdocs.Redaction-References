---
title: "TextReplacement"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "テキスト置換情報を表します。"
type: docs
weight: 33
url: /ja/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

テキスト置換情報を表します。

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | TextReplacement クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getIndex()](#getIndex--) | ソース文字列内で一致したテキストのインデックスを取得します。 |
|
|  | [getOriginalText()](#getOriginalText--) | 元の一致文字列を取得します。 |
|
|  | [getReplacement()](#getReplacement--) | OriginalText を置き換える文字列を取得します。 |
|
|  | [toString()](#toString--) | テキスト置換の説明とその位置を提供します。 |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


TextReplacement クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | インデックス | int | ソース文字列内で一致したテキストのインデックス |
|
|  | 元の | java.lang.String | 元の一致文字列 |
|
|  | 置換 | java.lang.String | ソース文字列で OriginalText を置き換える文字列 |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


ソース文字列内で一致したテキストのインデックスを取得します。


**Returns:**
int - ソース文字列内で一致したテキストのインデックスです。

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


元の一致文字列を取得します。


**Returns:**
java.lang.String - 元の一致文字列です。

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


OriginalText を置き換える文字列を取得します。


**Returns:**
java.lang.String - OriginalText を置き換える文字列です。

### toString() {#toString--}
```
public String toString()
```


テキスト置換の説明とその位置を提供します。


**Returns:**
java.lang.String - 置換の説明

