---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "適用する特定のリダクションのセットを含むサニタイズポリシーを表します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

適用する特定の編集のセットを含むサニタイズポリシーを表します。

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | Redaction ポリシーの新しいインスタンスを作成します。 |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | 特定のリダクションリストを使用して Redaction ポリシーの新しいインスタンスを作成します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | 完全に構成された配列を取得します |
Redaction
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | インスタンスをロードします |
RedactionPolicy
ファイルパスから。
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | インスタンスをロードします |
RedactionPolicy
ストリームから。
|
|  | [save(String filePath)](#save-java.lang.String-) | リダクションポリシーをファイルに保存します。 |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | リダクションポリシーをストリームに保存します。 |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Redaction ポリシーの新しいインスタンスを作成します。


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


特定のリダクションリストを使用して Redaction ポリシーの新しいインスタンスを作成します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | ポリシー用のリダクション配列 |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


完全に構成された配列を取得します
Redaction
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - 完全に構成された Redaction 派生クラスの配列。

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


インスタンスをロードします
RedactionPolicy
ファイルパスから。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | XML ファイルへのパス |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


インスタンスをロードします
RedactionPolicy
ストリームから。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | input | java.io.InputStream | XML構成を含むストリーム |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


リダクションポリシーをファイルに保存します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパス。 |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


リダクションポリシーをストリームに保存します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 出力 | java.io.OutputStream | ポリシーを保存する対象ストリーム |
|

