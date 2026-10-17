---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belge meta verisinin en yaygın türlerinin bir listesini temsil eder."
type: docs
weight: 640
url: /tr/net/groupdocs.redaction.redactions/metadatafilters/
---
## MetadataFilters enumeration

Belge meta verisinin en yaygın türlerinin bir listesini temsil eder.

```csharp
[Flags]
public enum MetadataFilters
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Boş filtre ayarı, hiçbir meta veri öğesiyle eşleşmez. |
| Author | `1` | Belgenin yazarı. |
| Category | `2` | Belgenin kategorisi. |
| Comments | `4` | Belge için yorum. |
| Company | `8` | Yazarın şirketi. |
| ContentStatus | `10` | İçerik durumu. |
| CreatedTime | `20` | Oluşturulma zamanı. |
| HyperlinkBase | `40` | Köprü temeli. |
| LastPrinted | `80` | Son yazdırma tarihi ve saati. |
| LastSavedBy | `100` | Kullanıcı tarafından son kaydedilen. |
| LastSavedTime | `400` | Son kaydedilen tarih ve saat. |
| NameOfApplication | `800` | Belgenin oluşturulduğu uygulamanın adı. |
| Manager | `1000` | Yazarın yöneticisinin adı. |
| RevisionNumber | `2000` | Revizyon numarası. |
| Subject | `4000` | Belgenin konusu. |
| Template | `8000` | Belge şablonu adı. |
| Title | `10000` | Belge başlığı. |
| TotalEditingTime | `20000` | Toplam düzenleme süresi. |
| Version | `40000` | Belgenin sürümü. |
| Description | `80000` | Belgenin açıklaması. |
| Keywords | `100000` | Belgenin anahtar kelimeleri. |
| ContentType | `200000` | İçerik türü. |
| All | `7FFFFFFF` | Metaveri öğelerinin tüm türleri. |

### Açıklamalar

**Learn more**

* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
