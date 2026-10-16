---
title: "FileType"
second_title: "GroupDocs.Redaction für .NET API-Referenz"
description: "Stellt einen Dateityp dar. Bietet Methoden, um eine Liste aller von GroupDocs.Redaction unterstützten Dateitypen zu erhalten, den Dateityp anhand der Erweiterung zu erkennen usw."
type: docs
weight: 90
url: /de/net/groupdocs.redaction/filetype/
---
## FileType class

Stellt einen Dateityp dar. Bietet Methoden, um eine Liste aller von GroupDocs.Redaction unterstützten Dateitypen zu erhalten, den Dateityp anhand der Erweiterung zu erkennen usw.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Bitmap-Bilddatei (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Kommagetrennte Werte-Datei (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | DjVu-Bild (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word-Dokument (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML-Makroaktiviertes Dokument (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML-Dokument (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word-Dokumentvorlage (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML-Makroaktivierte Dokumentvorlage (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML-Dokumentvorlage (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Grafik-Austauschformat-Datei (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Hypertext-Auszeichnungssprache-Datei (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Hypertext-Auszeichnungssprache-Datei (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 Kernbilddatei (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG-Bild (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG-Bild (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | Protokolldatei (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Markdown-Dokumentationsdatei (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers-Tabellenkalkulation (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument-Präsentation (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument-Tabellenkalkulation (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument-Textdokument (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | OpenDocument-Präsentationsvorlage (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument-Tabellenkalkulationsvorlage (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument-Dokumentvorlage (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Portable Document Format-Datei (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Portable Network Graphic (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | PowerPoint Open XML Makro-aktivierte Präsentationsvorlage (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | PowerPoint Open XML Präsentationsvorlage (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | PowerPoint Diashow (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | PowerPoint Open XML Makro-aktivierte Folie (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | PowerPoint Open XML Diashow (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint Präsentation (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | PowerPoint Open XML Makro-aktivierte Präsentation |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML Präsentation (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Rich Text Format-Datei (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | Tabulatorgetrennte Werte-Datei (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Tagged Image File (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Tagged Image File Format (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Tabulatorgetrennte Werte-Datei (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Nur-Text-Datei (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Stellt einen unbekannten Dateityp dar. |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | WebP-Bild (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel-Tabellenkalkulation (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel-Binär-Tabellenkalkulation (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML Makro-aktivierte Tabellenkalkulation (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML Tabellenkalkulation (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | Excel-Vorlage (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | Excel Open XML Makro-aktivierte Tabellenkalkulationsvorlage (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | Excel Open XML Tabellenkalkulationsvorlage (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Ermittelt den Dateinamensuffix (einschließlich des Punktes "."), zum Beispiel ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Ermittelt den Dateitypnamen, zum Beispiel "Microsoft Word Document". |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Ordnet Dateierweiterungen dem Dateityp zu. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Bestimmt, ob der aktuelle [`FileType`](../filetype) derselbe ist wie das angegebene [`FileType`](../filetype)-Objekt. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Bestimmt, ob der aktuelle [`FileType`](../filetype) derselbe ist wie das angegebene Objekt. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Gibt den Hashcode für das aktuelle [`FileType`](../filetype)-Objekt zurück. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Gibt eine Zeichenkette zurück, die das aktuelle Objekt darstellt. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Ruft unterstützte Dateitypen ab |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Bestimmt, ob zwei [`FileType`](../filetype)-Objekte identisch sind. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Bestimmt, ob zwei [`FileType`](../filetype)-Objekte nicht identisch sind. |

### Hinweise

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Siehe auch

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
