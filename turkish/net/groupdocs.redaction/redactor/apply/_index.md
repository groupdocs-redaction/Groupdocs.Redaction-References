---
title: "Uygula"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belgeye bir redaksiyon uygular."
type: docs
weight: 20
url: /tr/net/groupdocs.redaction/redactor/apply/
---
## Apply(Redaction) {#apply}

Belgeye bir redaksiyon uygular.

```csharp
public RedactorChangeLog Apply(Redaction redaction)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| redaction | Redaction | Uygulamak için bir [`Redaction`](../../redaction) örneği |

### Dönüş Değeri

Bu durumda başarı veya başarısızlık ve hata mesajı

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

### Ayrıca Bakınız

* class [RedactorChangeLog](../../redactorchangelog)
* class [Redaction](../../redaction)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Apply(Redaction[]) {#apply_2}

Belgeye bir dizi redaksiyon uygular.

```csharp
public RedactorChangeLog Apply(Redaction[] redactions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kırpmalar | Redaction[] | Uygulanacak redaksiyonların bir dizisi |

### Dönüş Değeri

Bu durumda başarı veya başarısızlık ve hata mesajı

### Örnekler

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

### Ayrıca Bakınız

* class [RedactorChangeLog](../../redactorchangelog)
* class [Redaction](../../redaction)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Apply(RedactionPolicy) {#apply_1}

Belgeye bir redaksiyon politikası uygular.

```csharp
public RedactorChangeLog Apply(RedactionPolicy policy)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| policy | RedactionPolicy | Kırpma politikası |

### Dönüş Değeri

Bu durumda başarı veya başarısızlık ve hata mesajı

### Örnekler

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

### Ayrıca Bakınız

* class [RedactorChangeLog](../../redactorchangelog)
* class [RedactionPolicy](../../redactionpolicy)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
