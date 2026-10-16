---
title: "FileType"
second_title: "GroupDocs.Redaction 适用于 .NET 的 API 参考"
description: "表示文件类型。提供方法以获取 GroupDocs.Redaction 支持的所有文件类型列表、通过扩展名检测文件类型等。"
type: docs
weight: 90
url: /zh/net/groupdocs.redaction/filetype/
---
## FileType class

表示一种文件类型。提供获取 GroupDocs.Redaction 支持的所有文件类型列表、通过扩展名检测文件类型等方法。

```csharp
public sealed class FileType : IEquatable<FileType>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | 位图图像文件 (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | 逗号分隔值文件 (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | DjVu 图像 (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word 文档 (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML 启用宏的文档 (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML 文档 (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word 文档模板 (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML 启用宏的文档模板 (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML 文档模板 (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | 图形交换格式文件 (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | 超文本标记语言文件 (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | 超文本标记语言文件 (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 核心图像文件 (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG 图像 (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG 图像 (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | 日志文件 (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Markdown 文档文件 (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers 电子表格 (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument 演示文稿 (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument 电子表格 (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument 文本文档 (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | OpenDocument 演示文稿模板 (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument 电子表格模板 (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument 文档模板 (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | 可移植文档格式文件 (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | 可移植网络图形 (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | PowerPoint Open XML 宏启用演示文稿模板 (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | PowerPoint Open XML 演示文稿模板 (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | PowerPoint 幻灯片放映 (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | PowerPoint Open XML 宏启用幻灯片 (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | PowerPoint Open XML 幻灯片放映 (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint 演示文稿 (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | PowerPoint Open XML 宏启用演示文稿 |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML 演示文稿 (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | 富文本格式文件 (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | 制表符分隔值文件 (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | 标记图像文件 (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | 标记图像文件格式 (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | 制表符分隔值文件 (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | 纯文本文件 (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | 表示未知文件类型。 |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | WebP 图像 (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel 电子表格 (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel 二进制电子表格 (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML 宏启用电子表格 (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML 电子表格 (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | Excel 模板 (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | Excel Open XML 宏启用电子表格模板 (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | Excel Open XML 电子表格模板 (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | 获取文件名后缀（包括句点 "."），例如 ".doc"。 |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | 获取文件类型名称，例如 "Microsoft Word Document"。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | 将文件扩展名映射到文件类型。 |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | 确定当前[`FileType`](../filetype)是否与指定的[`FileType`](../filetype)对象相同。 |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | 确定当前[`FileType`](../filetype)是否与指定的对象相同。 |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | 返回当前[`FileType`](../filetype)对象的哈希码。 |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | 返回表示当前对象的字符串。 |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | 检索受支持的文件类型 |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | 确定两个[`FileType`](../filetype)对象是否相同。 |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | 确定两个[`FileType`](../filetype)对象是否不相同。 |

### 备注

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### 另见

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
