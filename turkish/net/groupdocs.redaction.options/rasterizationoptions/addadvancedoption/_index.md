---
title: "AddAdvancedOption"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Uygulanacak bir gelişmiş rasterizasyon seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz."
type: docs
weight: 70
url: /tr/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Uygulanacak bir gelişmiş rasterizasyon seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Seçilen efekt türü (gri tonlama, kenarlık vb.) hakkında bilgi sağlar |

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

### Ayrıca Bakınız

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Uygulanacak bir gelişmiş rasterizasyon seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Seçilen efekt türü (gri tonlama, kenarlık vb.) hakkında bilgi sağlar |
| parameters | Dictionary`2 | Verilen efekt için parametreler, örneğin dönüş açısı |

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

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
