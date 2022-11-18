---
title: FileType
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Bir dosya türünü temsil eder. GroupDocs.Redaction tarafından desteklenen tüm dosya türlerinin bir listesini elde etmek dosya türünü uzantıya göre algılamak vb. için yöntemler sağlar.
type: docs
weight: 90
url: /tr/net/groupdocs.redaction/filetype/
---
## FileType class

Bir dosya türünü temsil eder. GroupDocs.Redaction tarafından desteklenen tüm dosya türlerinin bir listesini elde etmek, dosya türünü uzantıya göre algılamak vb. için yöntemler sağlar.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Bit Eşlem Görüntü Dosyası (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Virgülle Ayrılmış Değerler Dosyası (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word Belgesi (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Açık XML Makro Etkin Belge (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Açık XML Belgesi (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word Belgesi Şablonu (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Açık XML Makro Etkin Belge Şablonu (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Açık XML Belge Şablonu (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Grafik Değişim Formatı Dosyası (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Köprü Metni İşaretleme Dili Dosyası (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Köprü Metni İşaretleme Dili Dosyası (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 Çekirdek Görüntü Dosyası (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG Resmi (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG Resmi (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | İşaretleme Dokümantasyon Dosyası (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numaraları Elektronik Tablosu (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument Sunumu (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument Elektronik Tablosu (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument Metin Belgesi (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument Elektronik Tablo Şablonu (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument Belge Şablonu (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Taşınabilir Belge Biçimi Dosyası (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Taşınabilir Ağ Grafiği (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint Sunumu (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Açık XML Sunumu (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Zengin Metin Biçimi Dosyası (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Etiketli Resim Dosyası (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Etiketli Görüntü Dosyası Formatı (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Sekmeyle Ayrılmış Değerler Dosyası (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Düz Metin Dosyası (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Bilinmeyen dosya türünü temsil eder. |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel Elektronik Tablosu (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel İkili Hesap Tablosu (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Açık XML Makro Etkin Elektronik Tablo (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Açık XML Elektronik Tablosu (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Dosya adı son ekini ("." Noktası dahil) alır, örneğin ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Dosya türü adını alır, örneğin "Microsoft Word Belgesi". |

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Dosya uzantısını dosya türüyle eşler. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Mevcut olup olmadığını belirler.[`FileType`](../filetype) belirtilenle aynı[`FileType`](../filetype) nesne. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Mevcut olup olmadığını belirler.[`FileType`](../filetype) belirtilen nesneyle aynı. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Mevcut için hash kodunu döndürür[`FileType`](../filetype) nesne. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Geçerli nesneyi temsil eden bir dize döndürür. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Desteklenen dosya türlerini alır |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | İki olup olmadığını belirler[`FileType`](../filetype) nesneler aynıdır. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | İki olup olmadığını belirler[`FileType`](../filetype) nesneler aynı değil. |

### Notlar

**Daha fazla bilgi edin**

* [Desteklenen Belge Biçimleri](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Desteklenen dosya biçimlerini edinin](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Dosya bilgilerini al](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Ayrıca bakınız

* ad alanı [GroupDocs.Redaction](../../groupdocs.redaction)
* toplantı [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
