---
title: FileType
second_title: GroupDocs.Redaction for .NET API リファレンス
description: ファイルの種類を表します GroupDocs.Redaction でサポートされているすべてのファイル タイプのリストを取得するメソッド拡張子でファイル タイプを検出するメソッドなどを提供します
type: docs
weight: 90
url: /ja/net/groupdocs.redaction/filetype/
---
## FileType class

ファイルの種類を表します。 GroupDocs.Redaction でサポートされているすべてのファイル タイプのリストを取得するメソッド、拡張子でファイル タイプを検出するメソッドなどを提供します。

```csharp
public sealed class FileType : IEquatable<FileType>
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | ビットマップ イメージ ファイル (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | カンマ区切り値ファイル (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word ドキュメント (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML マクロ有効ドキュメント (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML ドキュメント (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word ドキュメント テンプレート (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML マクロ有効ドキュメント テンプレート (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML ドキュメント テンプレート (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | グラフィカル インターチェンジ フォーマット ファイル (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | ハイパーテキスト マークアップ言語ファイル (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | ハイパーテキスト マークアップ言語ファイル (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 コア イメージ ファイル (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG 画像 (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG 画像 (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | マークダウン ドキュメント ファイル (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers スプレッドシート (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument プレゼンテーション (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument スプレッドシート (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument テキスト ドキュメント (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument スプレッドシート テンプレート (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument ドキュメント テンプレート (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Portable Document Format ファイル (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | ポータブル ネットワーク グラフィック (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint プレゼンテーション (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML プレゼンテーション (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | リッチ テキスト形式ファイル (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | タグ付き画像ファイル (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | タグ付き画像ファイル形式 (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | タブ区切り値ファイル (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | プレーン テキスト ファイル (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | 不明なファイル タイプを表します。 |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel スプレッドシート (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel バイナリ スプレッドシート (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML マクロ有効スプレッドシート (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML スプレッドシート (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | ファイル名のサフィックス (ピリオド "." を含む) を取得します (例: ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | ファイルの種類の名前を取得します (例: "Microsoft Word Document". |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | ファイル拡張子をファイル タイプにマップします。 |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | 現在の[`FileType`](../filetype)指定と同じです[`FileType`](../filetype)object. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | 現在の[`FileType`](../filetype)指定されたオブジェクトと同じです. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | 現在のハッシュ コードを返します。[`FileType`](../filetype)object. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | 現在のオブジェクトを表す文字列を返します。 |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | サポートされているファイル タイプを取得します |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | 2 つの[`FileType`](../filetype)オブジェクトは同じです. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | 2 つの[`FileType`](../filetype)オブジェクトは同じではありません. |

### 備考

**もっと詳しく知る**

* [サポートされているドキュメント形式](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [サポートされているファイル形式を取得する](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [ファイル情報を取得する](https://docs.groupdocs.com/redaction/net/get-file-info/)

### 関連項目

* 名前空間 [GroupDocs.Redaction](../../groupdocs.redaction)
* 組み立て [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
