---
title: FileType
second_title: GroupDocs.Redaction for .NET API 参考
description: 表示文件类型提供获取 GroupDocs.Redaction 支持的所有文件类型列表按扩展名检测文件类型等方法
type: docs
weight: 90
url: /zh/net/groupdocs.redaction/filetype/
---
## FileType class

表示文件类型。提供获取 GroupDocs.Redaction 支持的所有文件类型列表、按扩展名检测文件类型等方法。

```csharp
public sealed class FileType : IEquatable<FileType>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | 位图图像文件 (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | 逗号分隔值文件 (.csv) |
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
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Markdown 文档文件 (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple 数字电子表格 (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument 演示文稿 (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument 电子表格 (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument 文本文档 (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument 电子表格模板 (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument 文档模板 (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | 可移植文档格式文件 (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | 便携式网络图形 (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint 演示文稿 (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML 演示文稿 (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | 富文本格式文件 (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | 标记图像文件 (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | 标记图像文件格式 (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | 制表符分隔值文件 (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | 纯文本文件 (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | 表示未知文件类型。 |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel 电子表格 (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel 二进制电子表格 (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML 启用宏的电子表格 (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML 电子表格 (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | 获取文件名后缀（包括句点“.”），例如“.doc”. |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | 获取文件类型名称，例如“Microsoft Word 文档”。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | 将文件扩展名映射到文件类型。 |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | 判断当前是否[`FileType`](../filetype)与指定的相同[`FileType`](../filetype)对象. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | 判断当前是否[`FileType`](../filetype)与指定对象相同。 |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | 返回当前的哈希码[`FileType`](../filetype)对象. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | 返回代表当前对象的字符串。 |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | 检索支持的文件类型 |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | 判断两个[`FileType`](../filetype)对象是相同的。 |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | 判断两个[`FileType`](../filetype)对象不一样。 |

### 评论

**学到更多**

* [支持的文档格式](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [获取支持的文件格式](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [获取文件信息](https://docs.groupdocs.com/redaction/net/get-file-info/)

### 也可以看看

* 命名空间 [GroupDocs.Redaction](../../groupdocs.redaction)
* 部件 [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
