---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een sanitatiebeleid voor dat een reeks specifieke redacties bevat die moeten worden toegepast."
type: docs
weight: 500
url: /nl/net/groupdocs.redaction/redactionpolicy/
---
## RedactionPolicy class

Stelt een sanitatiebeleid voor, dat een reeks specifieke redacties bevat die moeten worden toegepast.

```csharp
public class RedactionPolicy
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [RedactionPolicy](redactionpolicy#constructor)() | Creëert een nieuw exemplaar van Redaction policy. |
| [RedactionPolicy](redactionpolicy#constructor_1)(Redaction[]) | Creëert een nieuw exemplaar van Redaction policy met een specifieke lijst van redacties. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [Redactions](../../groupdocs.redaction/redactionpolicy/redactions) { get; } | Haalt een array op van volledig geconfigureerde [`Redaction`](../redaction)-afgeleide klassen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load)(Stream) | Laadt een instantie van [`RedactionPolicy`](../redactionpolicy) vanuit een stream. |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load_1)(string) | Laadt een instantie van [`RedactionPolicy`](../redactionpolicy) vanuit een bestandspad. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save)(Stream) | Slaat het redactiebeleid op naar een stream. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save_1)(string) | Slaat het redactiebeleid op naar een bestand. |

### Opmerkingen

**Learn more**

* More details about policies: [Use of redaction policies](https://docs.groupdocs.com/redaction/net/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)

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

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
