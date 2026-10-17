---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belge meta verisi redaksiyonları için temel soyut sınıfı temsil eder."
type: docs
weight: 650
url: /tr/net/groupdocs.redaction.redactions/metadataredaction/
---
## MetadataRedaction class

Belge meta verisi redaksiyonları için temel soyut sınıfı temsil eder.

```csharp
public abstract class MetadataRedaction : Redaction
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Redaction ve parametrelerini tanımlayan bir dize döndürür. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Tüm ya da belirli meta verileri (örneğin Yazar veya Şirket) seçmek için kullanılan filtreyi alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Redaction'ı verilen format örneğine uygular. |

### Açıklamalar

**Learn more**

* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Ayrıca Bakınız

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
