---
title: "FromExtension"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Dosya uzantısını dosya türüne eşler."
type: docs
weight: 500
url: /tr/net/groupdocs.redaction/filetype/fromextension/
---
## FileType.FromExtension method

Dosya uzantısını dosya türüne eşler.

```csharp
public static FileType FromExtension(string extension)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uzantı | String | Dosya uzantısı (nokta "." dahil). |

### Dönüş Değeri

Dosya türü destekleniyorsa onu döndürür, aksi takdirde varsayılan [`Unknown`](../unknown) dosya türünü döndürür.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | *extension* null veya boş bir dize olduğunda fırlatılır. |

### Ayrıca Bakınız

* class [FileType](../../filetype)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
