---
title: FileType
second_title: Riferimento API GroupDocs.Redaction per .NET
description: Rappresenta un tipo di file. Fornisce metodi per ottenere un elenco di tutti i tipi di file supportati da GroupDocs.Redaction rilevare il tipo di file per estensione ecc.
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
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | File con valori separati da virgola (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Documento Microsoft Word (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Documento con attivazione macro Word Open XML (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Apri documento XML (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Modello documento Word (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Modello documento con attivazione macro Word Open XML (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Modello documento Word Open XML (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | File in formato di interscambio grafico (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | File Hypertext Markup Language (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | File Hypertext Markup Language (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | File immagine principale JPEG 2000 (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | Immagine JPEG (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | Immagine JPEG (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | File di documentazione Markdown (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Foglio di calcolo dei numeri Apple (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | Presentazione OpenDocument (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | Foglio di calcolo OpenDocument (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument Documento di testo (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | Modello di foglio di calcolo OpenDocument (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | Modello documento OpenDocument (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | File in formato documento portatile (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Grafico di rete portatile (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | Presentazione PowerPoint (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | Presentazione PowerPoint Open XML (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | File in formato RTF (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | File immagine con tag (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Formato file immagine con tag (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | File dei valori separati da tabulazioni (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | File di testo semplice (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Rappresenta un tipo di file sconosciuto. |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Foglio di calcolo Excel (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Foglio di calcolo binario Excel (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML Foglio di calcolo con attivazione macro (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Apri foglio di calcolo XML (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Ottiene il suffisso del nome file (incluso il punto "."), ad esempio ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Ottiene il nome del tipo di file, ad esempio "Documento Microsoft Word". |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Associa l'estensione del file al tipo di file. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Determina se la corrente[`FileType`](../filetype) è uguale a quanto specificato[`FileType`](../filetype) oggetto. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Determina se la corrente[`FileType`](../filetype) è uguale all'oggetto specificato. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Restituisce il codice hash per la corrente[`FileType`](../filetype) oggetto. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Restituisce una stringa che rappresenta l'oggetto corrente. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Recupera i tipi di file supportati |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Determina se due[`FileType`](../filetype) gli oggetti sono gli stessi. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Determina se due[`FileType`](../filetype) gli oggetti non sono gli stessi. |

### Osservazioni

**Saperne di più**

* [Formati di documenti supportati](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Ottieni i formati di file supportati](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Ottieni informazioni sul file](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Guarda anche

* spazio dei nomi [GroupDocs.Redaction](../../groupdocs.redaction)
* assemblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
