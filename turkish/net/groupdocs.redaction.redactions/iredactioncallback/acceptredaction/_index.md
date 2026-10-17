---
title: "AcceptRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Bu çağrı, belgeye herhangi bir redaksiyon uygulanmadan hemen önce tetiklenir ve bunu kaydetmeye veya engellemeye olanak tanır."
type: docs
weight: 10
url: /tr/net/groupdocs.redaction.redactions/iredactioncallback/acceptredaction/
---
## IRedactionCallback.AcceptRedaction method

Bu çağrı, belgeye herhangi bir redaksiyon uygulanmadan hemen önce tetiklenir ve bunu kaydetmeye veya engellemeye olanak tanır.

```csharp
public bool AcceptRedaction(RedactionDescription description)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| açıklama | RedactionDescription | Belirli eşleşme türü, kriter, metin ve konum hakkında bilgi içerir |

### Dönüş Değeri

Belirli bir eşleşme redaksiyonunu kabul etmek için true, reddetmek için false döndürür

### Ayrıca Bakınız

* class [RedactionDescription](../../redactiondescription)
* interface [IRedactionCallback](../../iredactioncallback)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
