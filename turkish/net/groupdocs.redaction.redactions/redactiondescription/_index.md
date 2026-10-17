---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Redaksiyon sürecinde gerçekleştirilen tek bir değişiklik eylemi bilgisini temsil eder."
type: docs
weight: 720
url: /tr/net/groupdocs.redaction.redactions/redactiondescription/
---
## RedactionDescription class

Redaksiyon sürecinde gerçekleştirilen tek bir değişiklik eylemi bilgisini temsil eder.

```csharp
public class RedactionDescription
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RedactionDescription](redactiondescription#constructor_1)(RedactionType, RedactionActionType, string) | RedactionDescription sınıfının yeni bir örneğini, değiştirme bilgisi olmadan başlatır. |
| [RedactionDescription](redactiondescription#constructor)(RedactionType, RedactionActionType, RegionReplacementOptions, string) | RedactionDescription sınıfının yeni bir örneğini, görüntü alanı değiştirme bilgisiyle başlatır. |
| [RedactionDescription](redactiondescription#constructor_2)(RedactionType, RedactionActionType, string, TextReplacement) | RedactionDescription sınıfının yeni bir örneğini, değiştirme bilgisiyle başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActionType](../../groupdocs.redaction.redactions/redactiondescription/actiontype) { get; } | Kırpma işlemini alır: değiştirme, temizleme veya silme. |
| [Details](../../groupdocs.redaction.redactions/redactiondescription/details) { get; set; } | Kırpılan öğe için isteğe bağlı detay bilgilerini alır veya ayarlar. |
| [ImageAreaReplacement](../../groupdocs.redaction.redactions/redactiondescription/imageareareplacement) { get; } | Görüntü alanı kırpmaları için değiştirme bilgilerini alır, metin kırpmaları için null döndürür. |
| [OriginalText](../../groupdocs.redaction.redactions/redactiondescription/originaltext) { get; } | Herhangi bir ifade sağlanmışsa, eşleşen metni alır. |
| [RedactionType](../../groupdocs.redaction.redactions/redactiondescription/redactiontype) { get; } | Belgenin veri tipini alır - metin, meta veri veya ek açıklamalar. |
| [Replacement](../../groupdocs.redaction.redactions/redactiondescription/replacement) { get; } | Değiştirme bilgisini alır, null olabilir. |

### Açıklamalar

**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
