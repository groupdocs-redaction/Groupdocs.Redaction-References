---
title: FileType
second_title: GroupDocs.Redaction für .NET-API-Referenz
description: Repräsentiert einen Dateityp. Bietet Methoden zum Abrufen einer Liste aller von GroupDocs.Redaction unterstützten Dateitypen zum Erkennen des Dateityps anhand der Erweiterung usw.
type: docs
weight: 90
url: /de/net/groupdocs.redaction/filetype/
---
## FileType class

Repräsentiert einen Dateityp. Bietet Methoden zum Abrufen einer Liste aller von GroupDocs.Redaction unterstützten Dateitypen, zum Erkennen des Dateityps anhand der Erweiterung usw.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Bitmap-Bilddatei (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Kommagetrennte Wertedatei (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word-Dokument (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML-Dokument mit Makros (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML-Dokument (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word-Dokumentvorlage (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML-Dokumentvorlage mit Makros (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML-Dokumentvorlage (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Graphical Interchange Format-Datei (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Hypertext Markup Language-Datei (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Hypertext Markup Language-Datei (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 Core-Bilddatei (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG-Bild (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG-Bild (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Markdown-Dokumentationsdatei (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apfelzahlen-Tabelle (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument-Präsentation (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument-Tabelle (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument-Textdokument (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument-Tabellenvorlage (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument-Dokumentvorlage (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Portable Document Format-Datei (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Portable Netzwerkgrafik (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint-Präsentation (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML-Präsentation (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Datei im Rich-Text-Format (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Markierte Bilddatei (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Markiertes Bilddateiformat (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Tabulatorgetrennte Wertedatei (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Nur-Text-Datei (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | steht für unbekannten Dateityp. |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel-Tabelle (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel-Binärtabelle (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML-Makro-fähige Tabellenkalkulation (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML-Tabelle (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Ruft das Dateinamensuffix ab (einschließlich des Punktes "."), z. B. ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Ruft Dateitypnamen ab, zum Beispiel „Microsoft Word Document“. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Ordnet die Dateierweiterung dem Dateityp zu. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Bestimmt, ob der Strom[`FileType`](../filetype) ist genauso wie angegeben[`FileType`](../filetype) Objekt. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Bestimmt, ob der Strom[`FileType`](../filetype) ist das gleiche wie das angegebene Objekt. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Gibt den Hash-Code für den Strom zurück[`FileType`](../filetype) Objekt. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Gibt eine Zeichenfolge zurück, die das aktuelle Objekt darstellt. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Ruft unterstützte Dateitypen ab |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Bestimmt, ob zwei[`FileType`](../filetype) Objekte sind gleich. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Bestimmt, ob zwei[`FileType`](../filetype) Objekte sind nicht gleich. |

### Bemerkungen

**Mehr erfahren**

* [Unterstützte Dokumentformate](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Holen Sie sich unterstützte Dateiformate](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Dateiinformationen erhalten](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Siehe auch

* namensraum [GroupDocs.Redaction](../../groupdocs.redaction)
* Montage [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
