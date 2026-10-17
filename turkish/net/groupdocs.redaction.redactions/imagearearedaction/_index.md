---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Bir görüntü belgesinin belirli alanına renkli dikdörtgen yerleştiren bir redaksiyonu temsil eder."
type: docs
weight: 630
url: /tr/net/groupdocs.redaction.redactions/imagearearedaction/
---
## ImageAreaRedaction class

Bir görüntü belgesinin belirli alanına renkli dikdörtgen yerleştiren bir redaksiyonu temsil eder.

```csharp
public class ImageAreaRedaction : Redaction
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ImageAreaRedaction](imagearearedaction)(Point, RegionReplacementOptions) | Belirli bir alan boyutunu gizlemek için ImageAreaRedaction sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/imagearearedaction/description) { get; } | Redaction ve parametrelerini tanımlayan bir dize döndürür. |
| [Options](../../groupdocs.redaction.redactions/imagearearedaction/options) { get; } | Renk ve alan parametreleriyle [`RegionReplacementOptions`](../regionreplacementoptions) seçeneklerini alır. |
| [TopLeft](../../groupdocs.redaction.redactions/imagearearedaction/topleft) { get; } | Kaldırılacak alanın sol üst konumunu alır |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/imagearearedaction/applyto)(DocumentFormatInstance) | Redaction'ı verilen format örneğine uygular. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
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

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
