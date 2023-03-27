---
title: FileType
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: Merupakan jenis file. Menyediakan metode untuk mendapatkan daftar semua jenis file yang didukung oleh GroupDocs.Redaction mendeteksi jenis file dengan ekstensi dll.
type: docs
weight: 90
url: /id/net/groupdocs.redaction/filetype/
---
## FileType class

Merupakan jenis file. Menyediakan metode untuk mendapatkan daftar semua jenis file yang didukung oleh GroupDocs.Redaction, mendeteksi jenis file dengan ekstensi, dll.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Properti

| Nama | Keterangan |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | File Gambar Bitmap (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | File Nilai Terpisah Koma (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Dokumen Microsoft Word (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML Macro-Enabled Document (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Buka Dokumen XML (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Templat Dokumen Word (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML Macro-Enabled Document Template (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Templat Dokumen Word Open XML (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | File Format Pertukaran Grafis (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | File Bahasa Markup Hiperteks (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | File Bahasa Markup Hiperteks (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | File Gambar Inti JPEG 2000 (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | Gambar JPEG (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | Gambar JPEG (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | File Dokumentasi Markdown (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers Spreadsheet (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | Presentasi OpenDocument (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument Spreadsheet (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | Dokumen Teks OpenDocument (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | Templat Spreadsheet OpenDocument (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | Templat Dokumen OpenDocument (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | File Format Dokumen Portabel (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Grafik Jaringan Portabel (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | Presentasi PowerPoint (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML Presentation (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | File Format Teks Kaya (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | File Gambar yang Ditandai (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Format File Gambar yang Ditandai (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | File Nilai Terpisah Tab (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | File Teks Biasa (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Mewakili jenis file yang tidak diketahui. |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel Spreadsheet (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Lembar Kerja Biner Excel (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML Macro-Enabled Spreadsheet (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML Spreadsheet (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Mendapat akhiran nama file (termasuk titik "."), misalnya ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Mendapat nama jenis file, misalnya "Dokumen Microsoft Word". |

## Metode

| Nama | Keterangan |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Memetakan ekstensi file ke jenis file. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Menentukan apakah arus[`FileType`](../filetype) adalah sama dengan yang ditentukan[`FileType`](../filetype) objek. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Menentukan apakah arus[`FileType`](../filetype) sama dengan objek yang ditentukan. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Mengembalikan kode hash untuk saat ini[`FileType`](../filetype) objek. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Mengembalikan string yang mewakili objek saat ini. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Mengambil jenis file yang didukung |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Menentukan apakah dua[`FileType`](../filetype) objeknya sama. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Menentukan apakah dua[`FileType`](../filetype) objek tidak sama. |

### Perkataan

**Belajarlah lagi**

* [Format Dokumen yang Didukung](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Dapatkan format file yang didukung](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Dapatkan info file](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Lihat juga

* ruang nama [GroupDocs.Redaction](../../groupdocs.redaction)
* perakitan [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
