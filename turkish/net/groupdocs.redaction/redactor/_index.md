---
title: "Redactor"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belge redaksiyon sürecini kontrol eden, belgeleri açma, redakte etme ve kaydetme imkanı sağlayan ana sınıfı temsil eder."
type: docs
weight: 820
url: /tr/net/groupdocs.redaction/redactor/
---
## Redactor class

Belge redaksiyon sürecini kontrol eden, belgeleri açmaya, redakte etmeye ve kaydetmeye izin veren ana sınıfı temsil eder.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | [`Redactor`](../redactor) sınıfının akış kullanarak yeni bir örneğini başlatır. |
| [Redactor](redactor#constructor_3)(string) | [`Redactor`](../redactor) sınıfının dosya yolu kullanarak yeni bir örneğini başlatır. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Şifre korumalı bir belge için akış kullanarak [`Redactor`](../redactor) sınıfının yeni bir örneğini başlatır. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Şifre korumalı bir belge için yolunu kullanarak [`Redactor`](../redactor) sınıfının yeni bir örneğini başlatır. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Şifre korumalı bir belge için akış ve ayarları kullanarak [`Redactor`](../redactor) sınıfının yeni bir örneğini başlatır. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Şifre korumalı bir belge için yolunu ve ayarlarını kullanarak [`Redactor`](../redactor) sınıfının yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Belgeye bir redaksiyon uygular. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Belgeye bir redaksiyon politikası uygular. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Belgeye bir dizi redaksiyon uygular. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Kaynakları serbest bırakır. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Belirli sayfaların önizleme görüntülerini verilen bir görüntü formatında oluşturur. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Belge hakkında genel bilgileri alır - boyut, sayfa sayısı vb. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Belgeyi aşağıdaki seçeneklerle bir dosyaya kaydeder: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Belgeyi bir dosyaya kaydeder. |
| [Save](../../groupdocs.redaction/redactor/save#save_3)(Stream, SaveOptions) | Belgeyi belirtilen akışa kaydeder. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Örnekler

Aşağıdaki örnek, belgeye tek bir redaksiyon uygulanmasını gösterir.

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

Aşağıdaki örnek, belgeye bir redaksiyon listesi uygulanmasını gösterir.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... diğer redaksiyonlar
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false, en az bir redaksiyon başarısız olduysa
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

Aşağıdaki örnek, belirli bir gelen klasördeki tüm dosyalara bir kırpma politikası uygulamayı ve başarılı bir şekilde güncellenen dosyalar ile başarısız olanlar için bir giden klasöre kaydetmeyi gösterir.

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

Aşağıdaki örnek, LoadOptions kullanarak şifre korumalı belgelerin nasıl açılacağını gösterir.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Burada belge örneğini redaksiyonları gerçekleştirmek için kullanabiliriz
}
```

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

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
