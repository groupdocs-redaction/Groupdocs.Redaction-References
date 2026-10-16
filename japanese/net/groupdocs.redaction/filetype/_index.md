---
title: "FileType"
second_title: "GroupDocs.Redaction（.NET 用）API リファレンス"
description: "ファイルタイプを表します。GroupDocs.Redaction がサポートするすべてのファイルタイプの一覧を取得したり、拡張子でファイルタイプを検出したりするメソッドを提供します。"
type: docs
weight: 90
url: /ja/net/groupdocs.redaction/filetype/
---
## FileType class

ファイルタイプを表します。GroupDocs.Redaction がサポートするすべてのファイルタイプの一覧を取得したり、拡張子でファイルタイプを検出したりするメソッドを提供します。

```csharp
public sealed class FileType : IEquatable<FileType>
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | ビットマップ画像ファイル (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | カンマ区切り値ファイル (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | DjVu 画像 (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word 文書 (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML マクロ有効文書 (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML 文書 (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word 文書テンプレート (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML マクロ有効文書テンプレート (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML 文書テンプレート (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Graphics Interchange Format ファイル (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Hypertext Markup Language ファイル (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Hypertext Markup Language ファイル (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 コア画像ファイル (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG 画像 (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG 画像 (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | ログファイル (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Markdown ドキュメントファイル (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers スプレッドシート (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument プレゼンテーション (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument スプレッドシート (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument テキスト文書 (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | OpenDocument プレゼンテーションテンプレート (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument スプレッドシートテンプレート (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument 文書テンプレート (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Portable Document Format ファイル (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Portable Network Graphic (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | PowerPoint Open XML マクロ有効プレゼンテーションテンプレート (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | PowerPoint Open XML プレゼンテーションテンプレート (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | PowerPoint スライドショー (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | PowerPoint Open XML マクロ有効スライド (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | PowerPoint Open XML スライドショー (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint プレゼンテーション (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | PowerPoint Open XML マクロ有効プレゼンテーション |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML プレゼンテーション (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | リッチテキスト形式ファイル (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | タブ区切り値ファイル (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | タグ付き画像ファイル (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | タグ付き画像ファイル形式 (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | タブ区切り値ファイル (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | プレーンテキストファイル (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | 不明なファイルタイプを表します。 |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | WebP 画像 (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel スプレッドシート (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel バイナリスプレッドシート (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML マクロ有効スプレッドシート (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML スプレッドシート (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | Excel テンプレート (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | Excel Open XML マクロ有効スプレッドシートテンプレート (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | Excel Open XML スプレッドシートテンプレート (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | ファイル名のサフィックス（ピリオド「.」を含む）を取得します。例えば ".doc"。 |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | ファイルタイプ名を取得します。例えば "Microsoft Word Document"。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | ファイル拡張子をファイルタイプにマッピングします。 |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | 現在の[`FileType`](../filetype) が指定された[`FileType`](../filetype) オブジェクトと同じかどうかを判定します。 |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | 現在の[`FileType`](../filetype) が指定されたオブジェクトと同じかどうかを判定します。 |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | 現在の[`FileType`](../filetype) オブジェクトのハッシュコードを返します。 |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | 現在のオブジェクトを表す文字列を返します。 |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | サポートされているファイルタイプを取得します |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | 2つの[`FileType`](../filetype) オブジェクトが同じかどうかを判定します。 |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | 2つの[`FileType`](../filetype) オブジェクトが同じでないかどうかを判定します。 |

### 備考

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### 参照

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
