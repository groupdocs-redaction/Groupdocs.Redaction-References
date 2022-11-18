---
title: RedactionPolicy
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Uygulanacak bir dizi özel redaksiyon içeren bir temizleme politikasını temsil eder.
type: docs
weight: 400
url: /tr/net/groupdocs.redaction/redactionpolicy/
---
## RedactionPolicy class

Uygulanacak bir dizi özel redaksiyon içeren bir temizleme politikasını temsil eder.

```csharp
public class RedactionPolicy
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [RedactionPolicy](redactionpolicy#constructor)() | Redaksiyon politikasının yeni bir örneğini oluşturur. |
| [RedactionPolicy](redactionpolicy#constructor_1)(Redaction[]) | Belirli bir redaksiyon listesiyle Redaksiyon politikasının yeni bir örneğini oluşturur. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Redactions](../../groupdocs.redaction/redactionpolicy/redactions) { get; } | Tamamen yapılandırılmış bir dizi alır[`Redaction`](../redaction) -türetilmiş sınıflar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load)(Stream) | örneğini yükler[`RedactionPolicy`](../redactionpolicy) bir akıştan. |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load_1)(string) | örneğini yükler[`RedactionPolicy`](../redactionpolicy) bir dosya yolundan. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save)(Stream) | Redaksiyon politikasını bir akışa kaydeder. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save_1)(string) | Redaksiyon ilkesini bir dosyaya kaydeder. |

### Notlar

**Daha fazla bilgi edin**

* İlkeler hakkında daha fazla ayrıntı: [Redaksiyon politikalarının kullanımı](https://docs.groupdocs.com/redaction/net/use-redaction-policies/)
* Redaksiyonları uygulama hakkında daha fazla ayrıntı: [Redaksiyonun temelleri](https://docs.groupdocs.com/redaction/net/redaction-basics/)

### Örnekler

Aşağıdaki örnek, belirli bir gelen klasörü içindeki tüm dosyalara bir redaksiyon ilkesinin nasıl uygulanacağını ve başarıyla güncellenen dosyalar ve başarısız olanlar için giden klasörlerden birine nasıl kaydedileceğini gösterir.

Aşağıdaki örnek, tüm redaksiyon türleri için örnek yapılandırmalara sahip örnek bir XML ilke dosyası içerir.

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
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns = "http://www.groupdocs.com/redaction" >
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase = "dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <cellColumnRedaction regularExpression = "(foo)bar1" replacement="[red1]" columnIndex="1" worksheetIndex="2" /> 
  <cellColumnRedaction regularExpression = "(foo)bar2" replacement="[red2]" wokrsheetName="Sample" /> 
  
  <eraseMetadataRedaction filter = "All" />
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
 <annotationRedaction regularExpression = "(anno1)" replacement="foobar" />  
 <deleteAnnotationRedaction regularExpression = "(anno2)" />

 <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
 <imageAreaRedaction pointX = "110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy>
```

### Ayrıca bakınız

* ad alanı [GroupDocs.Redaction](../../groupdocs.redaction)
* toplantı [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->