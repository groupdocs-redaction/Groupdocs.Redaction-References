---
title: "FileType"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en filtyp. Tillhandahåller metoder för att hämta en lista över alla filtyper som stöds av GroupDocs.Redaction, upptäcka filtyp efter filändelse etc."
type: docs
weight: 90
url: /sv/net/groupdocs.redaction/filetype/
---
## FileType class

Representerar en filtyp. Tillhandahåller metoder för att hämta en lista över alla filtyper som stöds av GroupDocs.Redaction, upptäcka filtyp efter filändelse, etc.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Bitmap-bildfil (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Kommaseparerad värdefil (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | DjVu-bild (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word-dokument (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML-makroaktiverat dokument (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML-dokument (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word-dokumentmall (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML-makroaktiverad dokumentmall (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML-dokumentmall (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Graphics Interchange Format-fil (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Hypertext Markup Language-fil (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Hypertext Markup Language-fil (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 Core Image-fil (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG-bild (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG-bild (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | Loggfil (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Markdown-dokumentationsfil (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers-kalkylblad (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument-presentation (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument-kalkylblad (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument-textdokument (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | OpenDocument-presentationmall (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument-kalkylblads mall (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument-dokumentmall (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Portable Document Format-fil (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Portable Network Graphic-fil (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | PowerPoint Open XML-makroaktiverad presentationsmall (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | PowerPoint Open XML presentationsmall (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | PowerPoint bildspel (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | PowerPoint Open XML-makroaktiverad bild (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | PowerPoint Open XML bildspel (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint-presentation (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | PowerPoint Open XML-makroaktiverad presentation |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML-presentation (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Rich Text Format-fil (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | Tab-separerade värden-fil (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Taggad bildfil (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Taggat bildfilformat (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Tab-separerade värden-fil (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Oformaterad textfil (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Representerar okänd filtyp. |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | WebP-bild (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel-kalkylblad (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel binärt kalkylblad (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML-makroaktiverat kalkylblad (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML-kalkylblad (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | Excel-mall (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | Excel Open XML-makroaktiverad kalkylblads-mall (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | Excel Open XML kalkylblads-mall (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Hämtar filnamnsuffix (inklusive punkten "."), till exempel ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Hämtar filtypens namn, till exempel "Microsoft Word Document". |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Karterar filändelse till filtyp. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Bestämmer om den aktuella [`FileType`](../filetype) är densamma som det angivna [`FileType`](../filetype)-objektet. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Bestämmer om den aktuella [`FileType`](../filetype) är densamma som det angivna objektet. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Returnerar hashkoden för det aktuella [`FileType`](../filetype)-objektet. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Returnerar en sträng som representerar det aktuella objektet. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Hämtar stödda filtyper |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Bestämmer om två [`FileType`](../filetype)-objekt är desamma. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Bestämmer om två [`FileType`](../filetype)-objekt inte är desamma. |

### Anmärkningar

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Se även

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
