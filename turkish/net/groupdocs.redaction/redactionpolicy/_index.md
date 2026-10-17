---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Uygulanacak belirli kırpmaları içeren bir temizlik politikasını temsil eder."
type: docs
weight: 500
url: /tr/net/groupdocs.redaction/redactionpolicy/
---
## RedactionPolicy class

Uygulanacak belirli redaksiyon setini içeren bir temizlik politikasını temsil eder.

```csharp
public class RedactionPolicy
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RedactionPolicy](redactionpolicy#constructor)() | Redaction policy'nin yeni bir örneğini oluşturur. |
| [RedactionPolicy](redactionpolicy#constructor_1)(Redaction[]) | Redaction policy'yi belirli bir kırpma listesiyle yeni bir örnek olarak oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Redactions](../../groupdocs.redaction/redactionpolicy/redactions) { get; } | Tamamen yapılandırılmış [`Redaction`](../redaction) türevi sınıfların bir dizisini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load)(Stream) | [`RedactionPolicy`](../redactionpolicy) örneğini bir akıştan yükler. |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load_1)(string) | [`RedactionPolicy`](../redactionpolicy) örneğini bir dosya yolundan yükler. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save)(Stream) | Kırpma politikasını bir akışa kaydeder. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save_1)(string) | Kırpma politikasını bir dosyaya kaydeder. |

### Açıklamalar

**Learn more**

* More details about policies: [Use of redaction policies](https://docs.groupdocs.com/redaction/net/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)

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

Aşağıdaki örnek, tüm kırpma türleri için örnek yapılandırmalar içeren bir örnek XML politika dosyası içerir.

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

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
