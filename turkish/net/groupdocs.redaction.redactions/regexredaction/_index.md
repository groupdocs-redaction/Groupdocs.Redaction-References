---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Sağlanan düzenli ifadeyi eşleştirerek belgede metni arayan ve değiştiren bir metin redaksiyonunu temsil eder."
type: docs
weight: 750
url: /tr/net/groupdocs.redaction.redactions/regexredaction/
---
## RegexRedaction class

Sağlanan düzenli ifadeyi eşleştirerek belgede metni arayan ve değiştiren bir metin redaksiyonunu temsil eder.

```csharp
public class RegexRedaction : TextRedaction
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RegexRedaction](regexredaction#constructor_1)(Regex, ReplacementOptions) | RegexRedaction sınıfının yeni bir örneğini başlatır. |
| [RegexRedaction](regexredaction#constructor)(string, ReplacementOptions) | RegexRedaction sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Metin değiştirme türünü belirten [`ReplacementOptions`](../replacementoptions) örneğini alır. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Redaction ve parametrelerini tanımlayan bir dize döndürür. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Grafik içerikten metin çıkarmak için gerekli olan [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) uygulamasını alır veya ayarlar. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Eşleşecek düzenli ifadeyi alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/regexredaction/applyto)(DocumentFormatInstance) | Redaction'ı verilen format örneğine uygular. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Örnekler

Aşağıdaki örnek, düzenli ifade kullanarak metni değiştirmeyi gösterir.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
      // metinle değiştir
      redactor.Apply(new RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", new ReplacementOptions("[removed]")));
      // mavi katı dikdörtgenle değiştir
      redactor.Apply(new RegexRedaction(@"^\d+[,\.]{1}\d+$", new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)));
      redactor.Save();
    }
```

### Ayrıca Bakınız

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
