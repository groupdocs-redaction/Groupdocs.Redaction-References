---
title: FileType
second_title: GroupDocs.Redaction for .NET API Reference
description: Represents a file type. Provides methods to obtain a list of all file types supported by GroupDocs.Redaction detect file type by extension etc.
type: docs
weight: 90
url: /net/groupdocs.redaction/filetype/
---
## FileType class

Represents a file type. Provides methods to obtain a list of all file types supported by GroupDocs.Redaction, detect file type by extension, etc.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Properties

| Name | Description |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Bitmap Image File (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Comma Separated Values File (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word Document (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML Macro-Enabled Document (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML Document (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word Document Template (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML Macro-Enabled Document Template (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML Document Template (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Graphical Interchange Format File (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Hypertext Markup Language File (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Hypertext Markup Language File (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 Core Image File (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG Image (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG Image (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Markdown Documentation File (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers Spreadsheet (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument Presentation (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument Spreadsheet (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument Text Document (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument Spreadsheet Template (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument Document Template (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Portable Document Format File (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Portable Network Graphic (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint Presentation (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML Presentation (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Rich Text Format File (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Tagged Image File (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Tagged Image File Format (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Tab Separated Values File (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Plain Text File (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Represents unknown file type. |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel Spreadsheet (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel Binary Spreadsheet (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML Macro-Enabled Spreadsheet (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML Spreadsheet (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Gets filename suffix (including the period "."), for instance ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Gets file type name, for example "Microsoft Word Document". |

## Methods

| Name | Description |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Maps file extension to file type. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Determines whether the current [`FileType`](../filetype) is the same as specified [`FileType`](../filetype) object. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Determines whether the current [`FileType`](../filetype) is the same as specified object. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Returns the hash code for the current [`FileType`](../filetype) object. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Returns a string that represents the current object. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Retrieves supported file types |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Determines whether two [`FileType`](../filetype) objects are the same. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Determines whether two [`FileType`](../filetype) objects are not the same. |

### Remarks

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### See Also

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.redaction.dll -->
