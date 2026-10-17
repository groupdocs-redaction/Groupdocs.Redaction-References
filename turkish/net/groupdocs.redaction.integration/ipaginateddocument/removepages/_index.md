---
title: "RemovePages"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Başlangıç konumu ofseti ve sayısına bağlı olarak bir veya birden fazla sayfayı kaldırır."
type: docs
weight: 10
url: /tr/net/groupdocs.redaction.integration/ipaginateddocument/removepages/
---
## IPaginatedDocument.RemovePages method

Başlangıç konumu, offset ve sayıya bağlı olarak bir veya birden fazla sayfayı kaldırır.

```csharp
public RedactionResult RemovePages(PageSeekOrigin origin, int index, int count)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| origin | PageSeekOrigin | Belgenin başlangıç konumunu, başlangıcı ya da sonu arayın |
| index | Int32 | Başlangıç konumu indeksi (0 tabanlı) |
| count | Int32 | Kaldırılacak sayfa sayısı |

### Dönüş Değeri

Sayfa kaldırma redaksiyon sonucu

### Ayrıca Bakınız

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* enum [PageSeekOrigin](../../../groupdocs.redaction.redactions/pageseekorigin)
* interface [IPaginatedDocument](../../ipaginateddocument)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
