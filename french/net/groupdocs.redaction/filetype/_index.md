---
title: "FileType"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente un type de fichier. Fournit des méthodes pour obtenir une liste de tous les types de fichiers pris en charge par GroupDocs.Redaction, détecter le type de fichier par extension, etc."
type: docs
weight: 90
url: /fr/net/groupdocs.redaction/filetype/
---
## FileType class

Représente un type de fichier. Fournit des méthodes pour obtenir une liste de tous les types de fichiers pris en charge par GroupDocs.Redaction, détecter le type de fichier par extension, etc.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Propriétés

| Nom | Description |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Fichier image bitmap (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Fichier de valeurs séparées par des virgules (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | Image DjVu (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Document Microsoft Word (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Document Word Open XML avec macros (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Document Microsoft Word Open XML (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Modèle de document Word (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Modèle de document Word Open XML avec macros (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Modèle de document Word Open XML (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Fichier Graphical Interchange Format (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Fichier Hypertext Markup Language (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Fichier Hypertext Markup Language (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | Fichier JPEG 2000 Core Image (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | Image JPEG (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | Image JPEG (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | Fichier journal (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Fichier de documentation Markdown (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Feuille de calcul Apple Numbers (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | Présentation OpenDocument (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | Feuille de calcul OpenDocument (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | Document texte OpenDocument (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | Modèle de présentation OpenDocument (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | Modèle de feuille de calcul OpenDocument (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | Modèle de document OpenDocument (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Fichier Portable Document Format (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Graphique Portable Network (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | Modèle de présentation PowerPoint Open XML avec macros (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | Modèle de présentation PowerPoint Open XML (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | Diaporama PowerPoint (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | Diapositive PowerPoint Open XML avec macros (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | Diaporama PowerPoint Open XML (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | Présentation PowerPoint (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | Présentation PowerPoint Open XML avec macros |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | Présentation PowerPoint Open XML (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Fichier au format Rich Text Format (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | Fichier de valeurs séparées par des tabulations (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Fichier d'image Tagged Image File (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Format d'image Tagged Image File (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Fichier de valeurs séparées par des tabulations (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Fichier texte brut (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Représente un type de fichier inconnu. |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | Image WebP (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Feuille de calcul Excel (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Feuille de calcul binaire Excel (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Feuille de calcul Excel Open XML avec macros (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Feuille de calcul Microsoft Excel Open XML (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | Modèle Excel (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | Modèle de feuille de calcul Excel Open XML avec macros (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | Modèle de feuille de calcul Excel Open XML (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Obtient le suffixe du nom de fichier (y compris le point "."), par exemple ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Obtient le nom du type de fichier, par exemple "Microsoft Word Document". |

## Méthodes

| Nom | Description |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Mappe l'extension de fichier au type de fichier. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Détermine si le [`FileType`](../filetype) actuel est le même que l'objet [`FileType`](../filetype) spécifié. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Détermine si le [`FileType`](../filetype) actuel est le même que l'objet spécifié. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Renvoie le code de hachage pour l'objet [`FileType`](../filetype) actuel. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Renvoie une chaîne qui représente l'objet actuel. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Récupère les types de fichiers pris en charge |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Détermine si deux objets [`FileType`](../filetype) sont identiques. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Détermine si deux objets [`FileType`](../filetype) ne sont pas identiques. |

### Remarques

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Voir aussi

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
