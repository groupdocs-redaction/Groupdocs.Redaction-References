---
title: "FromName"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Bilinen bir rengin belirtilen adından bir renk oluşturur. Adı bilinen bir renk adı değilse bir istisna fırlatılır."
type: docs
weight: 1440
url: /tr/net/groupdocs.redaction.options.drawing/color/fromname/
---
## Color.FromName method

Bilinen bir rengin belirtilen adından renk oluşturur. *name* bilinen bir renk adı değilse, bir istisna fırlatılır.

```csharp
public static Color FromName(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Bilinen bir rengin adı, örneğin `Red` veya `Black`. |

### Dönüş Değeri

Adlandırılmış renk.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *name* `null`'dır. |
| ArgumentException | *name* bilinen bir renk adı değildir. |

### Ayrıca Bakınız

* struct [Color](../../color)
* namespace [GroupDocs.Redaction.Options.Drawing](../../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
