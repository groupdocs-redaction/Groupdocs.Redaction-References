---
title: "Load"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "RedactionPolicygroupdocs.redaction/redactionpolicy bir dosya yolundan bir örnek yükler."
type: docs
weight: 20
url: /tr/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

[`RedactionPolicy`](../../redactionpolicy) bir dosya yolundan bir örnek yükler.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | String | XML dosyasının yolu |

### Dönüş Değeri

Kırpma politikası

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

* class [RedactionPolicy](../../redactionpolicy)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

[`RedactionPolicy`](../../redactionpolicy) bir akıştan bir örnek yükler.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| input | Akış | XML yapılandırması içeren akış |

### Dönüş Değeri

Kırpma politikası

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

* class [RedactionPolicy](../../redactionpolicy)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
