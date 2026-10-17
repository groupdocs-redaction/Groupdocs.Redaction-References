---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Dosyaları PDF'ye dönüştürmek için seçenekler sağlar."
type: docs
weight: 420
url: /tr/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Dosyaları PDF'ye dönüştürmek için seçenekler sağlar.

```csharp
public class RasterizationOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Yeni bir örnek başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | PDF Uyumluluk seviyesini alır veya ayarlar. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Belgenin tüm sayfalarının görüntülere dönüştürülüp tek bir PDF dosyasına konulup konulmayacağını belirten bir değeri alır veya ayarlar. Varsayılan olarak TRUE, rasterizasyonu önlemek için FALSE olarak ayarlayın. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Gelişmiş rasterizasyon seçenekleri ayarlanmışsa true olan bir göstergeyi alır. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | PDF'ye dönüştürülecek sayfa sayısını alır veya ayarlar. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | PDF'ye dönüştürülecek ilk sayfanın (0 tabanlı) indeksini alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Uygulanacak bir gelişmiş rasterizasyon seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Uygulanacak bir gelişmiş rasterizasyon seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz. |

### Açıklamalar

**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Örnekler

Aşağıdaki örnek, rasterizasyon süreci için seçeneklerin nasıl ayarlanacağını gösterir.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // ilk slaytta hassas verileri kırp 
    
        var rasterizationOptions = new RasterizationOptions();
        rasterizationOptions.PageIndex = 0;
        rasterizationOptions.PageCount = 1;
        rasterizationOptions.Compliance = PdfComplianceLevel.PdfA1a;
        using (var stream = File.Open(Path.Combine(@"C:\Temp", "PresentationFirstSlide.pdf")))
        {
            redactor.Save(stream, rasterizationOptions);
        }
    }      
```

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
