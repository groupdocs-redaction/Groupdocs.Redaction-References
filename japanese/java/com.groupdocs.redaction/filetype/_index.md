---
title: "FileType"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "ファイルタイプを表します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

ファイルタイプを表します。GroupDocs.Redaction がサポートするすべてのファイルタイプの一覧を取得したり、拡張子からファイルタイプを検出したりするメソッドを提供します。

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | ファイルタイプ名を取得します。例: "Microsoft Word Document"。 |
|
|  | [getExtension()](#getExtension--) | ファイル名のサフィックス（ピリオド「.」を含む）を取得します。例: ".doc"。 |
|
|  | [getUnknown()](#getUnknown--) | 不明なファイルタイプを表します。 |
|
|  | [getTIF()](#getTIF--) | タグ付き画像ファイル (.tif) |
|
|  | [getTIFF()](#getTIFF--) | タグ付き画像ファイル形式 (.tiff) |
|
|  | [getJPG()](#getJPG--) | JPEG 画像 (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | JPEG 画像 (.jpeg) |
|
|  | [getPNG()](#getPNG--) | ポータブルネットワークグラフィック (.png) |
|
|  | [getGIF()](#getGIF--) | グラフィカル・インターチェンジ・フォーマット ファイル (.gif) |
|
|  | [getBMP()](#getBMP--) | ビットマップ画像ファイル (.bmp) |
|
|  | [getJP2()](#getJP2--) | JPEG 2000 コア画像ファイル (.jp2) |
|
|  | [getHTM()](#getHTM--) | ハイパーテキスト・マークアップ言語ファイル (.htm) |
|
|  | [getHTML()](#getHTML--) | ハイパーテキスト・マークアップ言語ファイル (.html) |
|
|  | [getPDF()](#getPDF--) | ポータブルドキュメントフォーマット ファイル (.pdf) |
|
|  | [getPPT()](#getPPT--) | PowerPoint プレゼンテーション (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | PowerPoint Open XML プレゼンテーション (.pptx) |
|
|  | [getODP()](#getODP--) | OpenDocument プレゼンテーション (.odp) |
|
|  | [getPOTX()](#getPOTX--) | PowerPoint Open XML プレゼンテーションテンプレート (.potx) |
|
|  | [getPOTM()](#getPOTM--) | PowerPoint Open XML マクロ有効プレゼンテーションテンプレート (.potm) |
|
|  | [getOTP()](#getOTP--) | OpenDocument プレゼンテーションテンプレート (.otp) |
|
|  | [getXLS()](#getXLS--) | Excel スプレッドシート (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Microsoft Excel Open XML スプレッドシート (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Excel Open XML マクロ有効スプレッドシート (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Excel バイナリ スプレッドシート (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Excel Open XML スプレッドシートテンプレート (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Excel Open XML マクロ有効スプレッドシートテンプレート (.xltm) |
|
|  | [getXLT()](#getXLT--) | Excel テンプレート (.xlt) |
|
|  | [getCSV()](#getCSV--) | カンマ区切り値ファイル (.csv) |
|
|  | [getTSV()](#getTSV--) | タブ区切り値ファイル (.tsv) |
|
|  | [getTAB()](#getTAB--) | タブ区切り値ファイル (.tab) |
|
|  | [getODS()](#getODS--) | OpenDocument スプレッドシート (.ods) |
|
|  | [getOTS()](#getOTS--) | OpenDocument スプレッドシートテンプレート (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Apple Numbers スプレッドシート (.numbers) |
|
|  | [getMD()](#getMD--) | Markdown ドキュメントファイル (.md) |
|
|  | [getDOC()](#getDOC--) | Microsoft Word 文書 (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Microsoft Word Open XML 文書 (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Word Open XML マクロ有効文書 (.docm) |
|
|  | [getDOT()](#getDOT--) | Word 文書テンプレート (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Word Open XML 文書テンプレート (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Word Open XML マクロ有効文書テンプレート (.dotm) |
|
|  | [getRTF()](#getRTF--) | リッチテキスト形式ファイル (.rtf) |
|
|  | [getTXT()](#getTXT--) | プレーンテキストファイル (.txt) |
|
|  | [getODT()](#getODT--) | OpenDocument テキスト文書 (.odt) |
|
|  | [getOTT()](#getOTT--) | OpenDocument 文書テンプレート (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | ファイル拡張子をファイルタイプにマッピングします。 |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | サポートされているファイルタイプを取得します |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | 現在のものかどうかを決定します |
FileType
指定されたものと同じです
FileType
オブジェクト。
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | 現在のものかどうかを決定します |
FileType
指定されたオブジェクトと同じです。
|
|  | [hashCode()](#hashCode--) | 現在のもののハッシュコードを返します |
FileType
オブジェクト。
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | 二つがかどうかを決定します |
FileType
オブジェクトは同じです。
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | 二つがかどうかを決定します |
FileType
オブジェクトは同じではありません。
|
|  | [toString()](#toString--) | 現在のオブジェクトを表す文字列を返します。 |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


ファイルタイプ名を取得します。例: "Microsoft Word Document"。


**Returns:**
java.lang.String - ファイルタイプ名（例: "Microsoft Word Document"）。

### getExtension() {#getExtension--}
```
public final String getExtension()
```


ファイル名のサフィックス（ピリオド「.」を含む）を取得します。例: ".doc"。


**Returns:**
java.lang.String - ファイル名のサフィックス（ピリオド「.」を含む）、例: ".doc"。

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


不明なファイルタイプを表します。


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIF() {#getTIF--}
```
public static FileType getTIF()
```


タグ付き画像ファイル (.tif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIFF() {#getTIFF--}
```
public static FileType getTIFF()
```


タグ付き画像ファイル形式 (.tiff)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPG() {#getJPG--}
```
public static FileType getJPG()
```


JPEG 画像 (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


JPEG 画像 (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


ポータブルネットワークグラフィック (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


グラフィカル・インターチェンジ・フォーマット ファイル (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


ビットマップ画像ファイル (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


JPEG 2000 コア画像ファイル (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


ハイパーテキスト・マークアップ言語ファイル (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


ハイパーテキスト・マークアップ言語ファイル (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


ポータブルドキュメントフォーマット ファイル (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


PowerPoint プレゼンテーション (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


PowerPoint Open XML プレゼンテーション (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


OpenDocument プレゼンテーション (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


PowerPoint Open XML プレゼンテーションテンプレート (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


PowerPoint Open XML マクロ有効プレゼンテーションテンプレート (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


OpenDocument プレゼンテーションテンプレート (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Excel スプレッドシート (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Microsoft Excel Open XML スプレッドシート (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Excel Open XML マクロ有効スプレッドシート (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Excel バイナリ スプレッドシート (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Excel Open XML スプレッドシートテンプレート (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Excel Open XML マクロ有効スプレッドシートテンプレート (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Excel テンプレート (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


カンマ区切り値ファイル (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


タブ区切り値ファイル (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


タブ区切り値ファイル (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


OpenDocument スプレッドシート (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


OpenDocument スプレッドシートテンプレート (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Apple Numbers スプレッドシート (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


Markdown ドキュメントファイル (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Microsoft Word 文書 (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Microsoft Word Open XML 文書 (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Word Open XML マクロ有効文書 (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Word 文書テンプレート (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Word Open XML 文書テンプレート (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Word Open XML マクロ有効文書テンプレート (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


リッチテキスト形式ファイル (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


プレーンテキストファイル (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


OpenDocument テキスト文書 (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


OpenDocument 文書テンプレート (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


ファイル拡張子をファイルタイプにマッピングします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 拡張子 | java.lang.String | ファイル拡張子（ピリオド「.」を含む）。 |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


サポートされているファイルタイプを取得します


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - サポートされているファイルタイプのシーケンスを返します

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


現在のものかどうかを決定します
FileType
指定されたものと同じです
FileType
オブジェクト。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | 現在の  FileType  オブジェクトと比較するオブジェクト。 |
|

**Returns:**
boolean - ```
true
```

if both  FileType  objects are the same; otherwise,

```
false
```


### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determines whether the current 
FileType
 is the same as specified object.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object to compare with the current  FileType  object.
 |

**Returns:**
boolean - ```
true
```

もし

```
obj
```

パラメーターが  FileType  であり、現在の  FileType  オブジェクトと同じ場合; それ以外の場合、

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


現在のもののハッシュコードを返します
FileType
オブジェクト。


**Returns:**
int - 現在の  FileType  オブジェクトのハッシュコード。

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


二つがかどうかを決定します
FileType
オブジェクトは同じです。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | 左側の  FileType  オブジェクト。 |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | 右側の  FileType  オブジェクト。 |
|

**Returns:**
boolean - ```
true
```

if both  FileType  objects are the same; otherwise,

```
false
```


### op_Inequality(FileType left, FileType right) {#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Inequality(FileType left, FileType right)
```


Determines whether two 
FileType
 objects are not the same.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| left | [FileType](../../com.groupdocs.redaction/filetype) | Left  FileType  object.
 |
| right | [FileType](../../com.groupdocs.redaction/filetype) | Right  FileType  object.
 |

**Returns:**
boolean - ```
true
```

両方の FileType オブジェクトが同じでない場合; それ以外の場合、

```
false
```


### toString() {#toString--}
```
public String toString()
```


現在のオブジェクトを表す文字列を返します。


**Returns:**
java.lang.String - 現在のオブジェクトを表す文字列です。

