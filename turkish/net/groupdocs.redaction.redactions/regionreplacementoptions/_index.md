---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Görüntü bölgesi değiştirme için renk ve alan parametrelerini temsil eder. Bkz ImageAreaRedaction./imagearearedaction."
type: docs
weight: 760
url: /tr/net/groupdocs.redaction.redactions/regionreplacementoptions/
---
## RegionReplacementOptions class

Görüntü bölgesi değiştirme için renk ve alan parametrelerini temsil eder. Bkz [`ImageAreaRedaction`](../imagearearedaction).

```csharp
public class RegionReplacementOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RegionReplacementOptions](regionreplacementoptions#constructor_1)(Color, Size) | RegionReplacementOptions sınıfının yeni bir örneğini başlatır. |
| [RegionReplacementOptions](regionreplacementoptions#constructor)(Color, Font, string) | Verilen metne uygun boyutta olan RegionReplacementOptions sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FillColor](../../groupdocs.redaction.redactions/regionreplacementoptions/fillcolor) { get; set; } | Redakte edilen alanı dolduracak rengi alır veya ayarlar. |
| [Size](../../groupdocs.redaction.redactions/regionreplacementoptions/size) { get; set; } | Dikdörtgenin genişliğini ve yüksekliğini alır veya ayarlar. |

### Açıklamalar

**Learn more**

* More details about image redactions: [Image redactions](https://docs.groupdocs.com/redaction/net/image-redactions/)

### Örnekler

Aşağıdaki örnek, görüntü içindeki bir alanı katı renkli bir dikdörtgenle değiştirmeyi gösterir.

```csharp
    using (Redactor redactor = new Redactor("D:\\test.jpg"))
    {
       GroupDocs.Redaction.Options.Drawing.Point samplePoint = new GroupDocs.Redaction.Options.Drawing.Point(516, 311);
       GroupDocs.Redaction.Options.Drawing.Size sampleSize = new GroupDocs.Redaction.Options.Drawing.Size(170, 35);
       RedactorChangeLog result = redactor.Apply(new ImageAreaRedaction(samplePoint,
                     new RegionReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue, sampleSize)));
       if (result.Status != RedactionStatus.Failed)
       {
          redactor.Save();
       };
    } 
```

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
