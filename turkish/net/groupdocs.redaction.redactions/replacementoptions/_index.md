---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Eşleşen metin değişimi için seçenekleri temsil eder."
type: docs
weight: 780
url: /tr/net/groupdocs.redaction.redactions/replacementoptions/
---
## ReplacementOptions class

Eşleşen metin değişimi için seçenekleri temsil eder.

```csharp
public class ReplacementOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ReplacementOptions](replacementoptions#constructor)(Color) | ReplacementOptions sınıfının yeni bir örneğini, renkli dikdörtgen seçeneğiyle başlatır. |
| [ReplacementOptions](replacementoptions#constructor_1)(string) | ReplacementOptions sınıfının yeni bir örneğini, değiştirme metni seçeneğiyle başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActionType](../../groupdocs.redaction.redactions/replacementoptions/actiontype) { get; } | Değiştirme eylemini alır: kutu çiz veya metni değiştir. |
| [BoxColor](../../groupdocs.redaction.redactions/replacementoptions/boxcolor) { get; set; } | DrawBox seçeneği için rengi alır veya ayarlar (aksi takdirde yok sayılır). |
| [CustomRedaction](../../groupdocs.redaction.redactions/replacementoptions/customredaction) { get; set; } | Kullanıcıların kendi redaksiyon mantıklarını tanımlamasına izin veren özel bir redaksiyon [`ICustomRedactionHandler`](../icustomredactionhandler) işleyicisini alır veya ayarlar. |
| [Filters](../../groupdocs.redaction.redactions/replacementoptions/filters) { get; set; } | Bu redaksiyonla uygulanacak filtreler dizisini alır veya ayarlar. |
| [Replacement](../../groupdocs.redaction.redactions/replacementoptions/replacement) { get; set; } | Metinsel değiştirme değerini alır veya ayarlar. |

### Açıklamalar

**Learn more**

* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
