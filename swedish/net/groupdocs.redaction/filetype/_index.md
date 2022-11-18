---
title: FileType
second_title: GroupDocs.Redaction för .NET API-referens
description: Representerar en filtyp. Tillhandahåller metoder för att få en lista över alla filtyper som stöds av GroupDocs.Redaction upptäcka filtyp efter förlängning etc.
type: docs
weight: 90
url: /sv/net/groupdocs.redaction/filetype/
---
## FileType class

Representerar en filtyp. Tillhandahåller metoder för att få en lista över alla filtyper som stöds av GroupDocs.Redaction, upptäcka filtyp efter förlängning, etc.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Bitmappsbildfil (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Kommaseparerade värdefil (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word-dokument (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML Macro-Enabled Document (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML-dokument (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word-dokumentmall (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML Makro-aktiverad dokumentmall (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML-dokumentmall (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Graphical Interchange Format File (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Hypertext Markup Language File (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Hypertext Markup Language File (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 Core Image File (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG-bild (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG-bild (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Markdown Documentation File (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers-kalkylblad (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument Presentation (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument Spreadsheet (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument Text Document (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument Spreadsheet Mall (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument Document Template (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Fil i portabelt dokumentformat (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Portable Network Graphic (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint-presentation (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML-presentation (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | RTF-fil (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Taggad bildfil (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Tagged Image File Format (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Flikseparerade värdefil (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Vanlig textfil (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Representerar okänd filtyp. |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel-kalkylblad (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel binärt kalkylblad (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML Macro-Enabled Kalkylblad (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel öppet XML-kalkylblad (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Får filnamnssuffix (inklusive perioden "."), till exempel ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Hämtar filtypsnamn, till exempel "Microsoft Word Document". |

## Metoder

| namn | Beskrivning |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Mappar filtillägget till filtyp. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Bestämmer om strömmen[`FileType`](../filetype) är samma som specificerat[`FileType`](../filetype) objekt. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Bestämmer om strömmen[`FileType`](../filetype) är samma som specificerat objekt. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Returnerar hashkoden för den aktuella[`FileType`](../filetype) objekt. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Returnerar en sträng som representerar det aktuella objektet. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Hämtar filtyper som stöds |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Bestämmer om två[`FileType`](../filetype) objekten är desamma. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Bestämmer om två[`FileType`](../filetype) objekt är inte samma sak. |

### Anmärkningar

**Läs mer**

* [Dokumentformat som stöds](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Få filformat som stöds](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Få filinformation](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Se även

* namnutrymme [GroupDocs.Redaction](../../groupdocs.redaction)
* hopsättning [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
