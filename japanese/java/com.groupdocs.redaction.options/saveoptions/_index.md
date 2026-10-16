---
title: "SaveOptions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "出力ファイル名の変更や、ドキュメントを画像ベースの PDF ラスタライズに変換するためのオプションを提供します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

出力ファイル名の変更や、ドキュメントを画像ベースの PDF（ラスタライズ）に変換するオプションを提供します。

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | デフォルトで新しいインスタンスを初期化します：PDF へのラスタライズ - false、サフィックスの追加 - false。 |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | 指定されたパラメータで新しいインスタンスを初期化します。 |
|
## フィールド

| フィールド | 説明 |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | デフォルトのサフィックス値を表します。値は "Redacted" です。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | 保存前にファイル名を変更する必要があるかどうかを示す値を取得します。 |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | 保存前にファイル名を変更する必要があるかどうかを示す値を設定します。 |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | 出力ファイル名のカスタムサフィックスを取得します。 |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | 出力ファイル名のカスタムサフィックスを設定します。 |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルにまとめる必要があるかどうかを示す値を取得します。 |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルにまとめる必要があるかどうかを示す値を設定します。 |
|
|  | [getRasterization()](#getRasterization--) | ラスタライズ設定を取得します。 |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | ワードプロセッシングの保存オプション。 |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


デフォルトで新しいインスタンスを初期化します：PDF へのラスタライズ - false、サフィックスの追加 - false。


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


指定されたパラメータで新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | True、ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルにまとめる必要がある場合 |
|
|  | suffix | java.lang.String | このテキストはファイル名の末尾に追加されます。空でない場合は AddSuffix も true に設定されます。 |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


デフォルトのサフィックス値を表します。値は "Redacted" です。


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


保存前にファイル名を変更する必要があるかどうかを示す値を取得します。デフォルトは false です。


**Returns:**
boolean - 保存前にファイル名を変更する必要があるかどうかを示す値です。デフォルトは false です。

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


保存前にファイル名を変更する必要があるかどうかを示す値を設定します。デフォルトは false です。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 保存前にファイル名を変更する必要があるかどうかを示す値です。デフォルトは false です。 |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


出力ファイル名のカスタムサフィックスを取得します。指定されていない場合は、
SaveSuffix
定数が使用されます。


**Returns:**
java.lang.String - 出力ファイル名のカスタムサフィックスです。指定されていない場合は、  SaveSuffix  定数が使用されます。

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


出力ファイル名のカスタムサフィックスを設定します。指定されていない場合は、
SaveSuffix
定数が使用されます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | 出力ファイル名のカスタムサフィックスです。指定されていない場合は、  SaveSuffix  定数が使用されます。 |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルにまとめる必要があるかどうかを示す値を取得します。


**Returns:**
boolean - ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルにまとめる必要があるかどうかを示す値です。

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルにまとめる必要があるかどうかを示す値を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | boolean | ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルにまとめる必要があるかどうかを示す値です。 |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


ラスタライズ設定を取得します。


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


ワードプロセッシングの保存オプション。


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
