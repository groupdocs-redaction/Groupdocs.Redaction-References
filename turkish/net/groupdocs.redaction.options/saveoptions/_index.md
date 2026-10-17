---
title: "SaveOptions"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Çıktı dosya adını değiştirme ve/veya belgeyi görüntü tabanlı PDF rasterlemesine dönüştürme seçenekleri sağlar."
type: docs
weight: 450
url: /tr/net/groupdocs.redaction.options/saveoptions/
---
## SaveOptions class

Çıktı dosya adını değiştirmek ve/veya belgeyi görüntü tabanlı PDF'ye (rasterleştirme) dönüştürmek için seçenekler sağlar.

```csharp
public class SaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SaveOptions](saveoptions#constructor)() | Varsayılanlarla yeni bir örnek başlatır: PDF'ye rasterleştir - false, ek sonek - false. |
| [SaveOptions](saveoptions#constructor_1)(bool, string) | Verilen parametrelerle yeni bir örnek başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AddSuffix](../../groupdocs.redaction.options/saveoptions/addsuffix) { get; set; } | Kaydetmeden önce dosya adının değiştirilip değiştirilmeyeceğini gösteren bir değeri alır veya ayarlar. Varsayılan olarak False. |
| [Rasterization](../../groupdocs.redaction.options/saveoptions/rasterization) { get; } | Rasterleştirme ayarlarını alır. |
| [RasterizeToPDF](../../groupdocs.redaction.options/saveoptions/rasterizetopdf) { get; set; } | Belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasına konulup konulmayacağını gösteren bir değeri alır veya ayarlar. |
| [RedactedFileSuffix](../../groupdocs.redaction.options/saveoptions/redactedfilesuffix) { get; set; } | Belirtilmezse, [`SaveSuffix`](./savesuffix) sabiti kullanılacaktır. |
| [WordprocessingSaveOptions](../../groupdocs.redaction.options/saveoptions/wordprocessingsaveoptions) { get; } | Kelime işlem belgelerine özgü kaydetme seçeneklerini alır. |

## Alanlar

| Ad | Açıklama |
| --- | --- |
| const [SaveSuffix](../../groupdocs.redaction.options/saveoptions/savesuffix) | Varsayılan sonek değerini temsil eder, bu "Redacted" dır. |

### Açıklamalar

**Learn more**

* [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
* [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
* [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
* [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

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

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
