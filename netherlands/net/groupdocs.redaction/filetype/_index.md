---
title: "FileType"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een bestandstype voor. Biedt methoden om een lijst te verkrijgen van alle bestandstypen die door GroupDocs.Redaction worden ondersteund, detecteert bestandstype op basis van extensie, enz."
type: docs
weight: 90
url: /nl/net/groupdocs.redaction/filetype/
---
## FileType class

Stelt een bestandstype voor. Biedt methoden om een lijst van alle bestandstypen die door GroupDocs.Redaction worden ondersteund op te halen, het bestandstype te detecteren op basis van extensie, enz.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Properties

| Naam | Beschrijving |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Bitmap‑afbeeldingsbestand (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Komma-gescheiden waardenbestand (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | DjVu-afbeelding (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word-document (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML-macro-ondersteund document (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML-document (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word-sjabloon (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML-macro-ondersteund sjabloon (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML-sjabloon (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Graphics Interchange Format-bestand (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Hypertext Markup Language-bestand (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Hypertext Markup Language-bestand (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 Core Image-bestand (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG-afbeelding (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG-afbeelding (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | Logbestand (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Markdown-documentatiebestand (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers-werkblad (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument-presentatie (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument-werkblad (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument-tekstdocument (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | OpenDocument-presentatiesjabloon (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument-werkbladsjabloon (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument-documentsjabloon (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Portable Document Format-bestand (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Portable Network Graphic-bestand (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | PowerPoint Open XML macro-ingeschakelde presentatiesjabloon (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | PowerPoint Open XML presentatiesjabloon (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | PowerPoint diavoorstelling (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | PowerPoint Open XML macro-ingeschakelde dia (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | PowerPoint Open XML diavoorstelling (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint-presentatie (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | PowerPoint Open XML macro-ingeschakelde presentatie |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML presentatie (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Rich Text Format-bestand (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | Tab-gescheiden waardenbestand (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Getagd afbeeldingsbestand (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Getagd afbeeldingsformaat (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Tab-gescheiden waardenbestand (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Platte tekstbestand (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Geeft onbekend bestandstype weer. |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | WebP-afbeelding (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel-werkblad (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel binair werkblad (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML macro-ingeschakeld werkblad (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML-werkblad (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | Excel-sjabloon (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | Excel Open XML macro-ingeschakelde werkbladsjabloon (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | Excel Open XML werkbladsjabloon (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Haalt bestandsnaamextensie op (inclusief de punt "."), bijvoorbeeld ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Haalt bestandssoortnaam op, bijvoorbeeld "Microsoft Word Document". |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Koppelt bestandsextensie aan bestandstype. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Bepaalt of de huidige [`FileType`](../filetype) hetzelfde is als het opgegeven [`FileType`](../filetype) object. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Bepaalt of de huidige [`FileType`](../filetype) hetzelfde is als het opgegeven object. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Retourneert de hashcode voor het huidige [`FileType`](../filetype) object. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Retourneert een tekenreeks die het huidige object vertegenwoordigt. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Haalt ondersteunde bestandstypen op |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Bepaalt of twee [`FileType`](../filetype) objecten hetzelfde zijn. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Bepaalt of twee [`FileType`](../filetype) objecten niet hetzelfde zijn. |

### Opmerkingen

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Zie ook

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
