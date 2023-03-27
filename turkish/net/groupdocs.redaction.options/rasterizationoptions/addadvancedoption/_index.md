---
title: AddAdvancedOption
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Uygulamak üzere gelişmiş bir rasterleştirme seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz.
type: docs
weight: 70
url: /tr/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Uygulamak üzere gelişmiş bir rasterleştirme seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Seçilen efekt türü (gri tonlama, kenarlık vb.) hakkında bilgi verir. |

### Örnekler

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

### Ayrıca bakınız

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* ad alanı [GroupDocs.Redaction.Options](../../rasterizationoptions)
* toplantı [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Uygulamak üzere gelişmiş bir rasterleştirme seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Seçilen efekt türü (gri tonlama, kenarlık vb.) hakkında bilgi verir. |
| parameters | Dictionary`2 | Dönme açısı gibi belirli bir etki için parametreler |

### Örnekler

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

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* ad alanı [GroupDocs.Redaction.Options](../../rasterizationoptions)
* toplantı [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
