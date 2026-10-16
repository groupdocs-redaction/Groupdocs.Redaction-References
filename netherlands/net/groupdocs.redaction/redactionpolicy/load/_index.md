---
title: "Laden"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Laadt een instantie van RedactionPolicygroupdocs.redaction/redactionpolicy vanaf een bestandspad."
type: docs
weight: 20
url: /nl/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

Laadt een instantie van [`RedactionPolicy`](../../redactionpolicy) vanaf een bestandspad.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Pad naar XML‑bestand |

### Retourwaarde

Redaction beleid

### Voorbeelden

Het volgende voorbeeld toont hoe een redactiebeleid toe te passen op alle bestanden in een opgegeven inkomende map, en op te slaan in een van de uitgaande mappen - voor succesvol bijgewerkte bestanden en voor mislukte bestanden.

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

Het volgende voorbeeld bevat een voorbeeld XML-beleidsbestand met voorbeeldconfiguraties voor alle soorten redacties.

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
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

Laadt een instantie van [`RedactionPolicy`](../../redactionpolicy) vanaf een stream.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| invoer | Stream | Stream met XML‑configuratie |

### Retourwaarde

Redaction beleid

### Voorbeelden

Het volgende voorbeeld toont hoe een redactiebeleid toe te passen op alle bestanden in een opgegeven inkomende map, en op te slaan in een van de uitgaande mappen - voor succesvol bijgewerkte bestanden en voor mislukte bestanden.

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

Het volgende voorbeeld bevat een voorbeeld XML-beleidsbestand met voorbeeldconfiguraties voor alle soorten redacties.

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
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
