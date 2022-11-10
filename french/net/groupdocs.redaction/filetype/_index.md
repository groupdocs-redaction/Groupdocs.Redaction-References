---
title: FileType
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Représente un type de fichier. Fournit des méthodes pour obtenir une liste de tous les types de fichiers pris en charge par GroupDocs.Redaction détecter le type de fichier par extension etc.
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

| Nom | La description |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Fichier image bitmap (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Fichier de valeurs séparées par des virgules (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Document Microsoft Word (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Document compatible avec les macros Word Open XML (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Document XML ouvert Microsoft Word (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Modèle de document Word (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Modèle de document compatible avec les macros Word Open XML (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Modèle de document XML ouvert Word (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Fichier de format d'échange graphique (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Fichier de langage de balisage hypertexte (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Fichier de langage de balisage hypertexte (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | Fichier d'image de base JPEG 2000 (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | Image JPEG (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | Image JPEG (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Fichier de documentation Markdown (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Feuille de calcul des nombres Apple (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | Présentation OpenDocument (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | Feuille de calcul OpenDocument (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | Document texte OpenDocument (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | Modèle de feuille de calcul OpenDocument (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | Modèle de document OpenDocument (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Fichier de format de document portable (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Graphique réseau portable (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | Présentation PowerPoint (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | Présentation XML ouverte PowerPoint (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Fichier au format RTF (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Fichier image balisé (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Format de fichier image tagué (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Fichier de valeurs séparées par des tabulations (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Fichier texte brut (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Représente un type de fichier inconnu. |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Feuille de calcul Excel (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Feuille de calcul binaire Excel (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Feuille de calcul Excel ouverte XML prenant en charge les macros (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Feuille de calcul Open XML Microsoft Excel (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Obtient le suffixe du nom de fichier (y compris le point "."), par exemple ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Obtient le nom du type de fichier, par exemple "Document Microsoft Word". |

## Méthodes

| Nom | La description |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Mappe l'extension de fichier au type de fichier. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Détermine si le courant[`FileType`](../filetype) est le même que celui spécifié[`FileType`](../filetype) objet. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Détermine si le courant[`FileType`](../filetype) est le même que l'objet spécifié. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Renvoie le code de hachage pour le courant[`FileType`](../filetype) objet. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Renvoie une chaîne qui représente l'objet actuel. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Récupère les types de fichiers pris en charge |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Détermine si deux[`FileType`](../filetype) les objets sont les mêmes. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Détermine si deux[`FileType`](../filetype) les objets ne sont pas les mêmes. |

### Remarques

**Apprendre encore plus**

* [Formats de documents pris en charge](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Obtenir les formats de fichiers pris en charge](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Obtenir des informations sur le fichier](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Voir également

* espace de noms [GroupDocs.Redaction](../../groupdocs.redaction)
* Assemblée [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
