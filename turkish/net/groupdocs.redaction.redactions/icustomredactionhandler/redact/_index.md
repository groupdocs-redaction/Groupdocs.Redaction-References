---
title: "Kırp"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belirli belge içeriğine özel redaksiyon uygular. Şu anda bu yalnızca PDF PageAreaRedactiongroupdocs.redaction.redactions/pagearearedaction için desteklenmektedir. Kullanıcılar, basit desen tabanlı yöntemlerden daha gelişmiş olabilecek AI tabanlı redaksiyon gibi kendi redaksiyon mantıklarını tanımlayabilir."
type: docs
weight: 10
url: /tr/net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
---
## ICustomRedactionHandler.Redact method

Belirli belge içeriğine özel redaksiyon uygular. Şu anda bu yalnızca PDF [`PageAreaRedaction`](../../pagearearedaction) için desteklenmektedir. Kullanıcılar, basit desen tabanlı yöntemlerden daha gelişmiş olabilecek AI tabanlı redaksiyon gibi kendi redaksiyon mantıklarını tanımlayabilir.

```csharp
public CustomRedactionResult Redact(CustomRedactionContext context)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bağlam | CustomRedactionContext | Redakte edilecek belge içeriğini ve ilgili üst verileri içerir. |

### Dönüş Değeri

Redaksiyonun uygulanıp uygulanmayacağını ve değiştirilmiş içeriği gösteren bir [`CustomRedactionResult`](../../customredactionresult).

### Ayrıca Bakınız

* class [CustomRedactionResult](../../customredactionresult)
* class [CustomRedactionContext](../../customredactioncontext)
* interface [ICustomRedactionHandler](../../icustomredactionhandler)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
