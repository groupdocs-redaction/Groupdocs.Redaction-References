---
title: "Save"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belgeyi aşağıdaki seçeneklerle bir dosyaya kaydeder AddSuffix  true RasterizeToPDF  true."
type: docs
weight: 60
url: /tr/net/groupdocs.redaction/redactor/save/
---
## Save() {#save}

Belgeyi aşağıdaki seçeneklerle bir dosyaya kaydeder: AddSuffix = true, RasterizeToPDF = true.

```csharp
public string Save()
```

### Dönüş Değeri

Kırpılmış belgeye yol

### Ayrıca Bakınız

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Save(SaveOptions) {#save_1}

Belgeyi bir dosyaya kaydeder.

```csharp
public string Save(SaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveOptions | SaveOptions | Sonek eklemek veya rasterleştirmek için seçenekler |

### Dönüş Değeri

Kırpılmış belgeye yol

### Örnekler

Aşağıdaki örnek, SaveOptions kullanarak bir belgeyi nasıl kaydedeceğinizi gösterir.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Belge redaksiyonu burada yer alır
       // ...
    
       // Belgeyi varsayılan seçeneklerle kaydet (sayfaları görüntülere dönüştür, PDF olarak kaydet)
       redactor.Save();
    
       // Belgeyi orijinal formatta, orijinal dosyanın üzerine yazarak kaydet
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Belgeyi orijinal formatta "*_Redacted.*" dosyasına kaydet
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Belgeyi rasterleştirme olmadan dosya adında "*_AnyText.*" (ör. "AnyText" yerine zaman damgası) olarak kaydet
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Ayrıca Bakınız

* class [SaveOptions](../../../groupdocs.redaction.options/saveoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Save(Stream, SaveOptions) {#save_3}

Belgeyi belirtilen akışa kaydeder.

```csharp
public void Save(Stream document, SaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| document | Akış | Hedef akış. |
| saveOptions | SaveOptions | Rasterleştirmeyi, çıktı dosya adı soneğini ve belgeye özgü kaydetme ayarlarını kontrol eden kaydetme seçenekleri. |

### Ayrıca Bakınız

* class [SaveOptions](../../../groupdocs.redaction.options/saveoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
