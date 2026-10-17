---
title: "PageAreaRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Sayfanın bir alanındaki metin görüntülerini ve ek açıklamaları etkileyen karmaşık bir metinsel redaksiyonu temsil eder."
type: docs
weight: 680
url: /tr/net/groupdocs.redaction.redactions/pagearearedaction/
---
## PageAreaRedaction class

Sayfanın bir alanındaki metin, görüntü ve açıklamaları etkileyen karmaşık bir metinsel redaksiyonu temsil eder.

```csharp
public class PageAreaRedaction : RegexRedaction
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PageAreaRedaction](pagearearedaction#constructor)(Regex, ReplacementOptions) | PageAreaRedaction sınıfının yeni bir örneğini başlatır. |
| [PageAreaRedaction](pagearearedaction#constructor_1)(Regex, ReplacementOptions, RegionReplacementOptions) | PageAreaRedaction sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Metin değiştirme türünü belirten [`ReplacementOptions`](../replacementoptions) örneğini alır. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Redaction ve parametrelerini tanımlayan bir dize döndürür. |
| [ImageOptions](../../groupdocs.redaction.redactions/pagearearedaction/imageoptions) { get; } | Renk ve alan parametreleriyle [`RegionReplacementOptions`](../regionreplacementoptions) seçeneklerini alır. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Grafik içerikten metin çıkarmak için gerekli olan [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) uygulamasını alır veya ayarlar. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Eşleşecek düzenli ifadeyi alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/pagearearedaction/applyto)(DocumentFormatInstance) | Redaction'ı verilen format örneğine uygular. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

### Ayrıca Bakınız

* class [RegexRedaction](../regexredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
