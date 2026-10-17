---
title: "IFixedFormatDocument"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "PDF veya sunumlar gibi sabit yapılı formatlara erişim için gerekli yöntemleri tanımlar."
type: docs
weight: 140
url: /tr/net/groupdocs.redaction.integration/ifixedformatdocument/
---
## IFixedFormatDocument interface

Sabit yapıdaki erişim formatları, örneğin PDF veya sunumlar için gereken yöntemleri tanımlar.

```csharp
public interface IFixedFormatDocument
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [LoadImages](../../groupdocs.redaction.integration/ifixedformatdocument/loadimages)(RedactionFilter[]) | Belge içinde bulunan, [`RedactionFilter`](../../groupdocs.redaction.redactions/redactionfilter) kümesiyle eşleşen raster görüntü örneklerinin bir dizisini yükler. |
| [RedactAnnotation](../../groupdocs.redaction.integration/ifixedformatdocument/redactannotation)(Regex, ReplacementOptions) | Belgedeki tüm ek açıklamalardaki eşleşen metni verilen seçeneklerle değiştirir. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
