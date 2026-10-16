---
title: "FileType"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta un tipo di file. Fornisce metodi per ottenere un elenco di tutti i tipi di file supportati da GroupDocs.Redaction, rilevare il tipo di file per estensione, ecc."
type: docs
weight: 90
url: /it/net/groupdocs.redaction/filetype/
---
## FileType class

Rappresenta un tipo di file. Fornisce metodi per ottenere un elenco di tutti i tipi di file supportati da GroupDocs.Redaction, rilevare il tipo di file per estensione, ecc.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | File immagine bitmap (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | File di valori separati da virgola (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | Immagine DjVu (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Documento Microsoft Word (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Documento Word Open XML con macro abilitata (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Documento Microsoft Word Open XML (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Modello di documento Word (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Modello di documento Word Open XML con macro abilitata (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Modello di documento Word Open XML (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | File Graphics Interchange Format (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | File di Hypertext Markup Language (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | File di Hypertext Markup Language (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | File immagine JPEG 2000 Core (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | Immagine JPEG (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | Immagine JPEG (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | File di registro (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | File di documentazione Markdown (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Foglio di calcolo Apple Numbers (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | Presentazione OpenDocument (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | Foglio di calcolo OpenDocument (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | Documento di testo OpenDocument (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | Modello di presentazione OpenDocument (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | Modello di foglio di calcolo OpenDocument (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | Modello di documento OpenDocument (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | File Portable Document Format (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Immagine Portable Network Graphics (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | Modello di presentazione PowerPoint Open XML con macro abilitata (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | Modello di presentazione PowerPoint Open XML (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | Presentazione diapositive PowerPoint (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | Diapositiva PowerPoint Open XML con macro abilitata (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | Presentazione diapositive PowerPoint Open XML (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | Presentazione PowerPoint (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | Presentazione PowerPoint Open XML con macro abilitata |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | Presentazione PowerPoint Open XML (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | File Rich Text Format (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | File di valori separati da tabulazione (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | File immagine con tag (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Formato file immagine con tag (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | File di valori separati da tabulazione (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | File di testo semplice (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Rappresenta un tipo di file sconosciuto. |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | Immagine WebP (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Foglio di calcolo Excel (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Foglio di calcolo binario Excel (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Foglio di calcolo Excel Open XML con macro abilitata (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Foglio di calcolo Microsoft Excel Open XML (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | Modello Excel (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | Modello di foglio di calcolo Excel Open XML con macro abilitata (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | Modello di foglio di calcolo Excel Open XML (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Ottiene il suffisso del nome file (incluso il punto "."), ad esempio ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Ottiene il nome del tipo di file, ad esempio "Microsoft Word Document". |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Mappa l'estensione del file al tipo di file. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Determina se il corrente [`FileType`](../filetype) è lo stesso dell'oggetto [`FileType`](../filetype) specificato. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Determina se il corrente [`FileType`](../filetype) è lo stesso dell'oggetto specificato. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Restituisce il codice hash per l'oggetto [`FileType`](../filetype) corrente. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Restituisce una stringa che rappresenta l'oggetto corrente. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Recupera i tipi di file supportati |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Determina se due oggetti [`FileType`](../filetype) sono gli stessi. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Determina se due oggetti [`FileType`](../filetype) non sono gli stessi. |

### Osservazioni

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Vedi anche

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
