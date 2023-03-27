---
title: FileType
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Vertegenwoordigt een bestandstype. Biedt methoden voor het verkrijgen van een lijst van alle bestandstypen die worden ondersteund door GroupDocs.Redaction het detecteren van bestandstypen op extensie enz.
type: docs
weight: 90
url: /nl/net/groupdocs.redaction/filetype/
---
## FileType class

Vertegenwoordigt een bestandstype. Biedt methoden voor het verkrijgen van een lijst van alle bestandstypen die worden ondersteund door GroupDocs.Redaction, het detecteren van bestandstypen op extensie, enz.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Bitmap afbeeldingsbestand (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | bestand met door komma's gescheiden waarden (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word-document (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML-document met ingeschakelde macro's (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML-document (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word-documentsjabloon (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML-documentsjabloon met ingeschakelde macro's (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML-documentsjabloon (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Bestand in grafische uitwisselingsindeling (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Hypertext Markup Language-bestand (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Hypertext Markup Language-bestand (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 kernbeeldbestand (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG-afbeelding (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG-afbeelding (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Markdown-documentatiebestand (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers-spreadsheet (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument Presentatie (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument Spreadsheet (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument tekstdocument (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument Spreadsheet-sjabloon (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument-documentsjabloon (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Draagbaar documentformaatbestand (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Draagbare netwerkafbeelding (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint-presentatie (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML-presentatie (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Rich Text Format-bestand (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Tagged afbeeldingsbestand (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Tagged afbeeldingsbestandsindeling (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Bestand met door tabs gescheiden waarden (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Platte tekstbestand (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Vertegenwoordigt onbekend bestandstype. |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel-werkblad (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel binaire spreadsheet (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML-spreadsheet met macro's (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML-werkblad (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Krijgt het achtervoegsel van de bestandsnaam (inclusief de punt "."), bijvoorbeeld ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Krijgt de naam van het bestandstype, bijvoorbeeld "Microsoft Word-document". |

## methoden

| Naam | Beschrijving |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Wijst bestandsextensie toe aan bestandstype. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Bepaalt of de stroom[`FileType`](../filetype) is hetzelfde als gespecificeerd[`FileType`](../filetype) object. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Bepaalt of de stroom[`FileType`](../filetype) is hetzelfde als gespecificeerd object. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Retourneert de hash-code voor de huidige[`FileType`](../filetype) object. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Retourneert een tekenreeks die het huidige object vertegenwoordigt. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Haalt ondersteunde bestandstypen op |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Bepaalt of twee[`FileType`](../filetype) objecten zijn hetzelfde. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Bepaalt of twee[`FileType`](../filetype) objecten zijn niet hetzelfde. |

### Opmerkingen

**Kom meer te weten**

* [Ondersteunde documentindelingen](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Download ondersteunde bestandsindelingen](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Bestandsinfo ophalen](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Zie ook

* naamruimte [GroupDocs.Redaction](../../groupdocs.redaction)
* montage [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
