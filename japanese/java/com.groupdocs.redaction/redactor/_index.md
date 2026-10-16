---
title: "Redactor"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "ドキュメントの赤字処理プロセスを制御し、開く、赤字処理、保存を行えるメインクラスを表します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

ドキュメントの編集プロセスを制御し、開く、編集する、保存することを可能にするメインクラスを表します。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | 新しいインスタンスを初期化します |
Redactor
ファイルパスを使用するクラスです。
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | 新しいインスタンスを初期化します |
Redactor
ストリームを使用するクラスです。
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | 新しいインスタンスを初期化します |
Redactor
パスワードで保護されたドキュメントのパスを使用するクラスです。
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | 新しいインスタンスを初期化します |
Redactor
パスワードで保護されたドキュメントのパスと設定を使用するクラスです。
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | 新しいインスタンスを初期化します |
Redactor
パスワードで保護されたドキュメントのストリームを使用するクラスです。
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | 新しいインスタンスを初期化します |
Redactor
パスワードで保護されたドキュメントのストリームと設定を使用するクラスです。
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [close()](#close--) | リソースを解放します。 |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | ドキュメントに赤字処理を適用します。 |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | ドキュメントに一連の赤字処理を適用します。 |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | ドキュメントに赤字ポリシーを適用します。 |
|
|  | [save()](#save--) | 次のオプションを使用してドキュメントをファイルに保存します: AddSuffix = true, RasterizeToPDF = true. |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | ドキュメントをファイルに保存します。 |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | ドキュメントをストリームに保存します。 |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | ドキュメントをストリームに保存します。 |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | カスタムロケーションを含めて、ドキュメントをストリームに保存します。 |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | 指定された画像形式で特定のページのプレビュー画像を生成します。 |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | ドキュメントの一般情報（サイズ、ページ数など）を取得します。 |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


新しいインスタンスを初期化します
Redactor
ファイルパスを使用するクラスです。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパス |


次の例は、ドキュメントをレダクション用に開く方法を示しています。

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
     // Here we can use document instance to perform redactions
 }
 
``` 
````

 |

### Redactor(InputStream document) {#Redactor-java.io.InputStream-}
```
public Redactor(InputStream document)
```


Initializes a new instance of 
Redactor
 class using stream.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source stream of the document


The following example demonstrates how to open a document from stream.

````

try (InputStream stream = new FileInputStream("C:\\sample.pdf"))
{
try (Redactor redactor = new Redactor(stream))
{
// ここでドキュメントインスタンスを使用してレダクションを実行できます
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


新しいインスタンスを初期化します
Redactor
パスワードで保護されたドキュメントのパスを使用するクラスです。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパス。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | パスワードを含むオプション。 |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


新しいインスタンスを初期化します
Redactor
パスワードで保護されたドキュメントのパスと設定を使用するクラスです。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパス。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | ファイル依存のオプション、パスワードを含む。 |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | レダクションプロセスのデフォルト設定。 |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


新しいインスタンスを初期化します
Redactor
パスワードで保護されたドキュメントのストリームを使用するクラスです。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | ドキュメント | java.io.InputStream | ソース入力ストリーム。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | パスワードを含むオプション。 |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


新しいインスタンスを初期化します
Redactor
パスワードで保護されたドキュメントのストリームと設定を使用するクラスです。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | ドキュメント | java.io.InputStream | ソース入力ストリーム。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | パスワードを含むオプション。 |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | レダクションプロセスのデフォルト設定。 |
|

### close() {#close--}
```
public final void close()
```


リソースを解放します。


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


ドキュメントに赤字処理を適用します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | 適用する Redaction のインスタンス |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


ドキュメントに一連の赤字処理を適用します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | 適用するレダクションの配列 |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


ドキュメントに赤字ポリシーを適用します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | レダクションポリシー |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


次のオプションを使用してドキュメントをファイルに保存します: AddSuffix = true, RasterizeToPDF = true.


**Returns:**
java.lang.String - レダクションされたドキュメントへのパス

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


ドキュメントをファイルに保存します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | サフィックスを追加またはラスタライズするオプション |
|

**Returns:**
java.lang.String - レダクションされたドキュメントへのパス

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


ドキュメントをストリームに保存します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | ドキュメント | java.io.OutputStream | ターゲットストリーム |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


ドキュメントをストリームに保存します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | ドキュメント | java.io.OutputStream | ターゲットストリーム |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | 保存オプション |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


カスタムロケーションを含めて、ドキュメントをストリームに保存します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | ドキュメント | java.io.OutputStream | ターゲットストリーム |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | ラスタライズするかしないか、そしてラスタライズ対象ページを指定するオプション |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


指定された画像形式で特定のページのプレビュー画像を生成します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | 画像プロパティとページ範囲設定 |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


ドキュメントの一般情報（サイズ、ページ数など）を取得します。


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

