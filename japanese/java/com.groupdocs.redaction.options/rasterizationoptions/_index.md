---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "ファイルを PDF に変換するためのオプションを提供します。"
type: docs
weight: 12
url: /ja/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

ファイルを PDF に変換するためのオプションを提供します。

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | 新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルにまとめる必要があるかどうかを示す値を取得します。 |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルにまとめる必要があるかどうかを示す値を設定します。 |
|
|  | [getPageIndex()](#getPageIndex--) | PDF に変換する最初のページのインデックス（0 ベース）を取得します。 |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | PDF に変換する最初のページのインデックス（0 ベース）を設定します。 |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | 初期化後に PageIndex プロパティが変更（設定）されたかどうかを示す値を取得します。 |
|
|  | [getPageCount()](#getPageCount--) | PDF に変換されるページ数を取得します。 |
|
|  | [setPageCount(int value)](#setPageCount-int-) | PDF に変換されるページ数を設定します。 |
|
|  | [isPageCountSet()](#isPageCountSet--) | 初期化後に PageCount プロパティが変更（設定）されたかどうかを示す値を取得します。 |
|
|  | [getCompliance()](#getCompliance--) | PDF コンプライアンスレベルを取得します。 |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | PDF コンプライアンスレベルを設定します。 |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | 高度なラスタライズオプションが設定されている場合に true になるインジケータを取得します。 |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | このメソッドを使用して、適用する高度なラスタライズオプションを登録できます。 |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | このメソッドを使用して、適用する高度なラスタライズオプションを登録できます。 |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


新しいインスタンスを初期化します。


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルに入れる必要があるかどうかを示す値を取得します。デフォルトは TRUE で、ラスタライズを回避するために FALSE に設定します。


**Returns:**
boolean - ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルに入れる必要があるかどうかを示す値です。デフォルトは TRUE で、ラスタライズを回避するために FALSE に設定します。

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルに入れるかどうかを示す値を設定します。デフォルトは TRUE で、ラスタライズを回避するために FALSE に設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | boolean | ドキュメント内のすべてのページを画像に変換し、単一の PDF ファイルに入れるかどうかを示す値です。デフォルトは TRUE で、ラスタライズを回避するために FALSE に設定します。 |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


PDF に変換する最初のページのインデックス（0 ベース）を取得します。


**Returns:**
int - PDF に変換する最初のページのインデックス（0 ベース）です。

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


PDF に変換する最初のページのインデックス（0 ベース）を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | int | PDF に変換する最初のページのインデックス（0 ベース）です。 |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


初期化後に PageIndex プロパティが変更（設定）されたかどうかを示す値を取得します。


**Returns:**
boolean - 初期化後に PageIndex プロパティが変更（設定）されたかどうかを示す値です。

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


PDF に変換されるページ数を取得します。


**Returns:**
int - PDF に変換されるページ数です。

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


PDF に変換されるページ数を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | int | PDF に変換されるページ数です。 |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


初期化後に PageCount プロパティが変更（設定）されたかどうかを示す値を取得します。


**Returns:**
boolean - 初期化後に PageCount プロパティが変更（設定）されたかどうかを示す値。

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


PDF コンプライアンスレベルを取得します。


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


PDF コンプライアンスレベルを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | PDF コンプライアンス レベル。 |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


高度なラスタライズオプションが設定されている場合に true になるインジケータを取得します。


**Returns:**
boolean - 高度なラスタライズオプションが設定されている場合に true になる指標。

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


このメソッドを使用して、適用する高度なラスタライズオプションを登録できます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | 選択されたエフェクトタイプ（グレースケール、ボーダーなど）に関する情報を提供します。 |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


このメソッドを使用して、適用する高度なラスタライズオプションを登録できます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | 選択されたエフェクトタイプ（グレースケール、ボーダーなど）に関する情報を提供します。 |
|
|  | パラメーター | java.util.HashMap<java.lang.String,java.lang.String> | 指定されたエフェクトのパラメーター（回転角度など） |
|

