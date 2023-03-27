---
title: Load
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: örneğini yüklerRedactionPolicygroupdocs.redaction/redactionpolicy bir dosya yolundan.
type: docs
weight: 20
url: /tr/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

örneğini yükler[`RedactionPolicy`](../../redactionpolicy) bir dosya yolundan.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | XML dosyasının yolu |

### Geri dönüş değeri

Redaksiyon politikası

### Örnekler

Aşağıdaki örnek, bir redaksiyon ilkesinin belirli bir gelen klasörü içindeki tüm dosyalara nasıl uygulanacağını ve başarıyla güncellenen dosyalar ve başarısız olanlar için giden klasörlerden birine nasıl kaydedileceğini gösterir.

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

* class [RedactionPolicy](../../redactionpolicy)
* ad alanı [GroupDocs.Redaction](../../redactionpolicy)
* toplantı [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

örneğini yükler[`RedactionPolicy`](../../redactionpolicy) bir akıştan.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| input | Stream | Akış içeren XML yapılandırması |

### Geri dönüş değeri

Redaksiyon politikası

### Örnekler

Aşağıdaki örnek, bir redaksiyon ilkesinin belirli bir gelen klasörü içindeki tüm dosyalara nasıl uygulanacağını ve başarıyla güncellenen dosyalar ve başarısız olanlar için giden klasörlerden birine nasıl kaydedileceğini gösterir.

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

* class [RedactionPolicy](../../redactionpolicy)
* ad alanı [GroupDocs.Redaction](../../redactionpolicy)
* toplantı [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
