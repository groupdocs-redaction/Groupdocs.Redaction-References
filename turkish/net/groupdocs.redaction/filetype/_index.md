---
title: "FileType"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Bir dosya türünü temsil eder. GroupDocs.Redaction tarafından desteklenen tüm dosya türlerinin listesini elde etmek, uzantıya göre dosya türünü tespit etmek vb. yöntemler sağlar."
type: docs
weight: 90
url: /tr/net/groupdocs.redaction/filetype/
---
## FileType class

Bir dosya türünü temsil eder. GroupDocs.Redaction tarafından desteklenen tüm dosya türlerinin listesini elde etmek, dosya türünü uzantıya göre tespit etmek vb. yöntemler sağlar.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Bitmap Görüntü Dosyası (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Virgülle Ayrılmış Değerler Dosyası (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | DjVu Görüntüsü (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word Belgesi (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML Makro Etkin Belgesi (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML Belgesi (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word Belge Şablonu (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML Makro Etkin Belge Şablonu (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML Belge Şablonu (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Grafik Değişim Biçimi Dosyası (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Hipermetin İşaretleme Dili Dosyası (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Hipermetin İşaretleme Dili Dosyası (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 Çekirdek Görüntü Dosyası (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG Görüntüsü (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG Görüntüsü (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | Günlük Dosyası (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Markdown Dokümantasyon Dosyası (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers Elektronik Tablosu (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument Sunumu (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument Elektronik Tablosu (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument Metin Belgesi (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | OpenDocument Sunum Şablonu (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument Elektronik Tablo Şablonu (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument Belge Şablonu (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Taşınabilir Belge Biçimi Dosyası (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Taşınabilir Ağ Grafiği (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | PowerPoint Open XML Makro Etkin Sunum Şablonu (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | PowerPoint Open XML Sunum Şablonu (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | PowerPoint Slayt Gösterisi (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | PowerPoint Open XML Makro Etkin Slayt (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | PowerPoint Open XML Slayt Gösterisi (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint Sunumu (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | PowerPoint Open XML Makro Etkin Sunum |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML Sunum (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Zengin Metin Biçimi Dosyası (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | Sekmeli Ayrılmış Değerler Dosyası (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Etiketli Görüntü Dosyası (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Etiketli Görüntü Dosyası Biçimi (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Sekmeli Ayrılmış Değerler Dosyası (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Düz Metin Dosyası (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Bilinmeyen dosya türünü temsil eder. |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | WebP Görüntüsü (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel Çalışma Sayfası (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel İkili Çalışma Sayfası (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML Makro Etkin Çalışma Sayfası (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML Çalışma Sayfası (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | Excel Şablonu (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | Excel Open XML Makro Etkin Çalışma Sayfası Şablonu (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | Excel Open XML Çalışma Sayfası Şablonu (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Dosya adı uzantısını alır (nokta "." dahil), örneğin ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Dosya türü adını alır, örneğin "Microsoft Word Document". |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Dosya uzantısını dosya türüne eşler. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Mevcut [`FileType`](../filetype) nesnesinin belirtilen [`FileType`](../filetype) nesnesiyle aynı olup olmadığını belirler. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Mevcut [`FileType`](../filetype) nesnesinin belirtilen nesneyle aynı olup olmadığını belirler. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Mevcut [`FileType`](../filetype) nesnesi için karma kodunu döndürür. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Mevcut nesneyi temsil eden bir dize döndürür. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Desteklenen dosya türlerini alır |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | İki [`FileType`](../filetype) nesnesinin aynı olup olmadığını belirler. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | İki [`FileType`](../filetype) nesnesinin aynı olmadığını belirler. |

### Açıklamalar

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
