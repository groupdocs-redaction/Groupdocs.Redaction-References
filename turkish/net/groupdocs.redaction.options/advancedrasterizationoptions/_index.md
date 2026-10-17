---
title: "AdvancedRasterizationOptions"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Uygulanacak gelişmiş rasterleştirme seçeneklerini yönetmek için bayrak sıralamasını tanımlar."
type: docs
weight: 290
url: /tr/net/groupdocs.redaction.options/advancedrasterizationoptions/
---
## AdvancedRasterizationOptions enumeration

Uygulanacak gelişmiş rasterleştirme seçeneklerini yönetmek için bayrak sıralamasını tanımlar.

```csharp
public enum AdvancedRasterizationOptions
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Uygulanacak gelişmiş seçenek yok. |
| Tilt | `1` | Rasterleştirilmiş görüntüyü rastgele bir açıya eğmek için eğin. |
| Noise | `2` | Rasterleştirilmiş sayfa görüntülerine rastgele lekeler ekle. |
| Border | `4` | Sayfa tarama etkisini taklit etmek için kenar çizgisi ekle. |
| Grayscale | `8` | Sayfa görüntülerini gri tonlamalı yaparak gri ton taramasını taklit et. |

### Örnekler

Aşağıdaki örnek, varsayılan ayarlarla gelişmiş rasterleştirme seçeneklerini nasıl uygulayacağınızı gösterir.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Belgeyi varsayılan seçeneklerle kaydet (sayfaları görüntülere dönüştür, PDF olarak kaydet)
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Grayscale);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt);
      redactor.Save(so);
    }
```

Aşağıdaki örnek, özel ayarlarla kenar gelişmiş rasterleştirme seçeneğini nasıl uygulayacağınızı gösterir.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Belgeyi özel bir kenarla kaydet
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

Aşağıdaki örnek, özel ayarlarla gürültü gelişmiş rasterleştirme seçeneğini nasıl uygulayacağınızı gösterir.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Belgeyi özel gürültü etkileri sayısı ve boyutu ile kaydedin
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

Aşağıdaki örnek, özel ayarlarla eğim gelişmiş rasterleştirme seçeneğinin nasıl uygulanacağını gösterir.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Belgeyi özel eğim etkisiyle kaydedin
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
