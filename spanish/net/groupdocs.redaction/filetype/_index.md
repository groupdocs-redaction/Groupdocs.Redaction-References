---
title: FileType
second_title: Referencia de API de GroupDocs.Redaction para .NET
description: Representa un tipo de archivo. Proporciona métodos para obtener una lista de todos los tipos de archivos compatibles con GroupDocs.Redaction detectar el tipo de archivo por extensión etc.
type: docs
weight: 90
url: /es/net/groupdocs.redaction/filetype/
---
## FileType class

Representa un tipo de archivo. Proporciona métodos para obtener una lista de todos los tipos de archivos compatibles con GroupDocs.Redaction, detectar el tipo de archivo por extensión, etc.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Archivo de imagen de mapa de bits (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Archivo de valores separados por comas (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Documento de Microsoft Word (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Documento Word Open XML habilitado para macros (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Documento XML abierto de Microsoft Word (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Plantilla de documento de Word (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Plantilla de documento Word Open XML habilitado para macros (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Plantilla de documento XML abierto de Word (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Archivo de formato de intercambio gráfico (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Archivo de lenguaje de marcado de hipertexto (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Archivo de lenguaje de marcado de hipertexto (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | Archivo de imagen principal JPEG 2000 (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | Imagen JPEG (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | Imagen JPEG (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Archivo de documentación de rebajas (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Hoja de cálculo de números de Apple (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | Presentación de documento abierto (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | Hoja de cálculo OpenDocument (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | Documento de texto OpenDocument (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | Plantilla de hoja de cálculo de OpenDocument (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | Plantilla de documento OpenDocument (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Archivo de formato de documento portátil (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Gráfico de red portátil (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | Presentación de PowerPoint (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | Presentación XML abierta de PowerPoint (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Archivo de formato de texto enriquecido (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Archivo de imagen etiquetado (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Formato de archivo de imagen etiquetada (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Archivo de valores separados por tabulaciones (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Archivo de texto sin formato (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Representa un tipo de archivo desconocido. |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Hoja de cálculo de Excel (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Hoja de cálculo binaria de Excel (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Hoja de cálculo Excel Open XML habilitada para macros (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Hoja de cálculo XML abierta de Microsoft Excel (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Obtiene el sufijo del nombre de archivo (incluido el punto "."), por ejemplo, ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Obtiene el nombre del tipo de archivo, por ejemplo, "Documento de Microsoft Word". |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Asigna la extensión del archivo al tipo de archivo. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Determina si la corriente[`FileType`](../filetype) es igual a lo especificado[`FileType`](../filetype) objeto. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Determina si la corriente[`FileType`](../filetype) es el mismo que el objeto especificado. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Devuelve el código hash para el actual[`FileType`](../filetype) objeto. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Devuelve una cadena que representa el objeto actual. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Recupera tipos de archivo admitidos |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Determina si dos[`FileType`](../filetype) los objetos son iguales. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Determina si dos[`FileType`](../filetype) los objetos no son iguales. |

### Observaciones

**Aprende más**

* [Formatos de documentos admitidos](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Obtener formatos de archivo compatibles](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Obtener información del archivo](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Ver también

* espacio de nombres [GroupDocs.Redaction](../../groupdocs.redaction)
* asamblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
