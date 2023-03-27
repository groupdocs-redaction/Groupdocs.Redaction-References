---
title: RasterizationOptions
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Dosyaları PDFye dönüştürmek için seçenekler sunar.
type: docs
weight: 350
url: /tr/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Dosyaları PDF'ye dönüştürmek için seçenekler sunar.

```csharp
public class RasterizationOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Yeni bir örneği başlatır. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | PDF Uyumluluk düzeyini alır veya ayarlar. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Belgedeki tüm sayfaların görüntülere dönüştürülmesi ve tek bir PDF dosyasına yerleştirilmesi gerekip gerekmediğini gösteren bir değer alır veya ayarlar. Varsayılan olarak DOĞRU, rasterleştirmeyi önlemek için YANLIŞ olarak ayarlayın. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Gelişmiş rasterleştirme seçenekleri ayarlanmışsa doğru olan bir gösterge alır. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | PDF'ye dönüştürülecek sayfa sayısını alır veya ayarlar. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | PDF'ye dönüştürmek için ilk sayfanın dizinini (0 tabanlı) alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Uygulamak üzere gelişmiş bir rasterleştirme seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Uygulamak üzere gelişmiş bir rasterleştirme seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz. |

### Notlar

**Daha fazla bilgi edin**

* Belgeyi rasterleştirilmiş bir PDF olarak kaydetme hakkında daha fazla ayrıntı: [Rasterleştirilmiş PDF'de kaydet](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* Rasterleştirme seçenekleri hakkında daha fazla ayrıntı: [Rasterleştirilmiş PDF için belirli sayfaları seçin](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Örnekler

Aşağıdaki örnek, rasterleştirme işlemi için seçeneklerin nasıl ayarlanacağını gösterir.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // ilk slayttaki hassas verileri reddet 
    
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

Aşağıdaki örnek, gelişmiş rasterleştirme seçeneklerinin varsayılan ayarlarla nasıl uygulanacağını gösterir.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Belgeyi varsayılan seçeneklerle kaydedin (sayfaları görüntülere dönüştürün, PDF olarak kaydedin)
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

Aşağıdaki örnek, kenarlık gelişmiş rasterleştirme seçeneğinin özel ayarlarla nasıl uygulanacağını gösterir.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Belgeyi özel bir kenarlıkla kaydedin
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

Aşağıdaki örnek, gürültü gelişmiş rasterleştirme seçeneğinin özel ayarlarla nasıl uygulanacağını gösterir.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Belgeyi gürültü efektlerinin özel sayısı ve boyutuyla kaydedin
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

Aşağıdaki örnek, özel ayarlarla tilt gelişmiş rasterleştirme seçeneğinin nasıl uygulanacağını gösterir.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Belgeyi özel eğim efektiyle kaydedin
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Ayrıca bakınız

* ad alanı [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* toplantı [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
