---
title: Redactor
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Belge düzeltme sürecini kontrol eden belgeleri açmaya düzeltmeye ve kaydetmeye izin veren bir ana sınıfı temsil eder.
type: docs
weight: 660
url: /tr/net/groupdocs.redaction/redactor/
---
## Redactor class

Belge düzeltme sürecini kontrol eden, belgeleri açmaya, düzeltmeye ve kaydetmeye izin veren bir ana sınıfı temsil eder.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Yeni bir örneğini başlatır[`Redactor`](../redactor) stream. kullanan sınıf |
| [Redactor](redactor#constructor_3)(string) | Yeni bir örneğini başlatır[`Redactor`](../redactor) dosya yolunu kullanan sınıf. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Yeni bir örneğini başlatır[`Redactor`](../redactor) stream. kullanan parola korumalı bir belge için sınıf |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Yeni bir örneğini başlatır[`Redactor`](../redactor) path. kullanan parola korumalı bir belge için sınıf |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Yeni bir örneğini başlatır[`Redactor`](../redactor)akış ve ayarları kullanan parola korumalı bir belge için sınıf. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Yeni bir örneğini başlatır[`Redactor`](../redactor) yolunu ve ayarlarını kullanan parola korumalı bir belge için sınıf. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Belgeye bir redaksiyon uygular. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Belgeye bir redaksiyon politikası uygular. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Belgeye bir dizi düzeltme uygular. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Kaynakları serbest bırakır. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Belirli sayfaların önizleme resimlerini belirli bir resim biçiminde oluşturur. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Belge hakkında genel bilgileri alır - boyut, sayfa sayısı, vb. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Belgeyi aşağıdaki seçeneklerle bir dosyaya kaydeder: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Belgeyi bir dosyaya kaydeder. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | Belgeyi, özel konum da dahil olmak üzere bir akışa kaydeder. |

### Notlar

**Daha fazla bilgi edin**

* Redaksiyonları uygulama hakkında daha fazla ayrıntı: [Redaksiyonun temelleri](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Daha gelişmiş redaksiyon konuları: [gelişmiş kullanım](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Örnekler

Aşağıdaki örnek, belgeye tek bir redaksiyonun uygulanmasını göstermektedir.

Aşağıdaki örnek, bir redaksiyon listesinin belgeye uygulanmasını göstermektedir.

Aşağıdaki örnek, bir redaksiyon ilkesinin belirli bir gelen klasörü içindeki tüm dosyalara nasıl uygulanacağını ve başarıyla güncellenen dosyalar ve başarısız olanlar için giden klasörlerden birine nasıl kaydedileceğini gösterir.

Aşağıdaki örnek, parola korumalı belgelerin LoadOptions kullanılarak nasıl açılacağını gösterir.

Aşağıdaki örnek, SaveOptions kullanılarak bir belgenin nasıl kaydedileceğini gösterir.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   RedactorChangeLog result = redactor.Apply(new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")));
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   var redactionList = new Redaction[] 
   {
      new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
      new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(System.Drawing.Color.Red)),
      new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
      new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(System.Drawing.Color.Blue)),
      // ... diğer düzeltmeler
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // yanlış, en az bir redaksiyon başarısız olursa
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
RedactionPolicy policy = RedactionPolicy.Load("RedactionPolicy.xml");
foreach (var fileEntry in Directory.GetFileNames("C:\\Inbound")) 
{
     using (Redactor redactor = new Redactor(Path.Combine("C:\\Inbound\\", fileEntry)))
     {
    	     RedactorChangeLog result = redactor.Apply(policy);
    	     String resultFolder = result.Status != RedactionStatus.Failed ? "C:\\Outbound\\Done\\" : "C:\\Outbound\\Failed\\";
    	     using (Stream fileStream = File.Open(Path.Combine(resultFolder, fileEntry), FileMode.Open, FileAccess.ReadWrite))
   	     {
               redactor.Save(fileStream, new RasterizationOptions() { Enabled = false });
   	     }        
     }
}   
```

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Burada redaksiyon yapmak için belge örneğini kullanabiliriz
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Belge redaksiyonu buraya gelir
       // ...
    
       // Belgeyi varsayılan seçeneklerle kaydedin (sayfaları görüntülere dönüştürün, PDF olarak kaydedin)
       redactor.Save();
    
       // Orijinal dosyanın üzerine yazarak belgeyi orijinal biçimde kaydedin
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Belgeyi orijinal formatta "*_Redacted.*" dosyasına kaydedin
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Belgeyi rasterleştirmeden dosya adında "*_AnyText.*" (örn. "AnyText" yerine zaman damgası) olarak kaydedin
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Ayrıca bakınız

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* ad alanı [GroupDocs.Redaction](../../groupdocs.redaction)
* toplantı [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
