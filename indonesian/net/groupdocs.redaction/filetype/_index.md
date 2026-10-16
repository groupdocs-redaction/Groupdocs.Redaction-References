---
title: "FileType"
second_title: "Referensi API GroupDocs.Redaction untuk .NET"
description: "Mewakili tipe file. Menyediakan metode untuk memperoleh daftar semua tipe file yang didukung oleh GroupDocs.Redaction, mendeteksi tipe file berdasarkan ekstensi, dll."
type: docs
weight: 90
url: /id/net/groupdocs.redaction/filetype/
---
## FileType class

Mewakili tipe file. Menyediakan metode untuk memperoleh daftar semua tipe file yang didukung oleh GroupDocs.Redaction, mendeteksi tipe file berdasarkan ekstensi, dll.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | File Gambar Bitmap (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | File Nilai yang Dipisahkan Koma (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | Gambar DjVu (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Dokumen Microsoft Word (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Dokumen Word Open XML yang Mendukung Makro (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Dokumen Microsoft Word Open XML (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Templat Dokumen Word (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Templat Dokumen Word Open XML yang Mendukung Makro (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Templat Dokumen Word Open XML (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | File Format Pertukaran Grafis (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Berkas Hypertext Markup Language (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Berkas Hypertext Markup Language (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | Berkas Gambar Inti JPEG 2000 (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | Gambar JPEG (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | Gambar JPEG (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | Berkas Log (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Berkas Dokumentasi Markdown (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Lembar Kerja Apple Numbers (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | Presentasi OpenDocument (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | Lembar Kerja OpenDocument (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | Dokumen Teks OpenDocument (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | Templat Presentasi OpenDocument (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | Templat Lembar Kerja OpenDocument (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | Templat Dokumen OpenDocument (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Berkas Format Dokumen Portabel (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Grafik Jaringan Portabel (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | Templat Presentasi PowerPoint Open XML yang Mendukung Makro (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | Templat Presentasi PowerPoint Open XML (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | Pertunjukan Slide PowerPoint (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | Slide PowerPoint Open XML yang Mendukung Makro (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | Pertunjukan Slide PowerPoint Open XML (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | Presentasi PowerPoint (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | Presentasi PowerPoint Open XML yang Mendukung Makro |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | Presentasi PowerPoint Open XML (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Berkas Rich Text Format (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | Berkas Nilai Dipisahkan Tab (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Berkas Gambar Bertanda (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Format Berkas Gambar Bertanda (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Berkas Nilai Dipisahkan Tab (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Berkas Teks Biasa (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Mewakili tipe berkas yang tidak diketahui. |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | Gambar WebP (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Lembar Kerja Excel (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Lembar Kerja Biner Excel (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Lembar Kerja Excel Open XML yang Mendukung Makro (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Lembar Kerja Microsoft Excel Open XML (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | Templat Excel (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | Templat Lembar Kerja Excel Open XML yang Mendukung Makro (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | Templat Lembar Kerja Excel Open XML (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Mendapatkan akhiran nama berkas (termasuk titik "."), misalnya ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Mendapatkan nama tipe berkas, misalnya "Microsoft Word Document". |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Memetakan ekstensi file ke tipe file. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Menentukan apakah [`FileType`](../filetype) saat ini sama dengan objek [`FileType`](../filetype) yang ditentukan. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Menentukan apakah [`FileType`](../filetype) saat ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Mengembalikan kode hash untuk objek [`FileType`](../filetype) saat ini. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Mengembalikan string yang merepresentasikan objek saat ini. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Mengambil tipe file yang didukung |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Menentukan apakah dua objek [`FileType`](../filetype) sama. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Menentukan apakah dua objek [`FileType`](../filetype) tidak sama. |

### Catatan

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Lihat Juga

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
