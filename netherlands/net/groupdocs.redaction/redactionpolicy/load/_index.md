---
title: Load
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Laadt een exemplaar vanRedactionPolicygroupdocs.redaction/redactionpolicy vanuit een bestandspad.
type: docs
weight: 20
url: /nl/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

Laadt een exemplaar van[`RedactionPolicy`](../../redactionpolicy) vanuit een bestandspad.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Pad naar XML-bestand |

### Winstwaarde

Redactiebeleid

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een redactiebeleid toepast op alle bestanden in een bepaalde inkomende map en opslaat in een van de uitgaande mappen - voor succesvol bijgewerkte bestanden en voor mislukte bestanden.

Het volgende voorbeeld bevat een voorbeeld van een XML-beleidsbestand met voorbeeldconfiguraties voor alle typen redactie.

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

### Zie ook

* class [RedactionPolicy](../../redactionpolicy)
* naamruimte [GroupDocs.Redaction](../../redactionpolicy)
* montage [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

Laadt een exemplaar van[`RedactionPolicy`](../../redactionpolicy) uit een stream.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| input | Stream | Stream met XML-configuratie |

### Winstwaarde

Redactiebeleid

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een redactiebeleid toepast op alle bestanden in een bepaalde inkomende map en opslaat in een van de uitgaande mappen - voor succesvol bijgewerkte bestanden en voor mislukte bestanden.

Het volgende voorbeeld bevat een voorbeeld van een XML-beleidsbestand met voorbeeldconfiguraties voor alle typen redactie.

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

### Zie ook

* class [RedactionPolicy](../../redactionpolicy)
* naamruimte [GroupDocs.Redaction](../../redactionpolicy)
* montage [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
