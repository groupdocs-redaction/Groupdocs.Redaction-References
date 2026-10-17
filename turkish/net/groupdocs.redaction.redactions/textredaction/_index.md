---
title: "TextRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belge metni redaksiyonları için temel soyut sınıfı temsil eder."
type: docs
weight: 800
url: /tr/net/groupdocs.redaction.redactions/textredaction/
---
## TextRedaction class

Belge metni redaksiyonları için temel soyut sınıfı temsil eder.

```csharp
public abstract class TextRedaction : Redaction
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Metin değiştirme türünü belirten [`ReplacementOptions`](../replacementoptions) örneğini alır. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Redaction ve parametrelerini tanımlayan bir dize döndürür. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Grafik içerikten metin çıkarmak için gerekli olan [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) uygulamasını alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| abstract [ApplyTo](../../groupdocs.redaction/redaction/applyto)(DocumentFormatInstance) | Redaction'ı verilen format örneğine uygular. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Ayrıca Bakınız

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
