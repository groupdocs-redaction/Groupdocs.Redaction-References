---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en saneringspolicy som innehåller en uppsättning specifika raderingar att tillämpa."
type: docs
weight: 500
url: /sv/net/groupdocs.redaction/redactionpolicy/
---
## RedactionPolicy class

Representerar en saneringspolicy som innehåller en uppsättning specifika raderingar att tillämpa.

```csharp
public class RedactionPolicy
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [RedactionPolicy](redactionpolicy#constructor)() | Skapar en ny instans av Redaction policy. |
| [RedactionPolicy](redactionpolicy#constructor_1)(Redaction[]) | Skapar en ny instans av Redaction policy med en specifik lista av raderingar. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Redactions](../../groupdocs.redaction/redactionpolicy/redactions) { get; } | Hämtar en array av fullt konfigurerade [`Redaction`](../redaction)-avledda klasser. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load)(Stream) | Laddar en instans av [`RedactionPolicy`](../redactionpolicy) från en ström. |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load_1)(string) | Laddar en instans av [`RedactionPolicy`](../redactionpolicy) från en filsökväg. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save)(Stream) | Sparar redigeringspolicyn till en ström. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save_1)(string) | Sparar redigeringspolicyn till en fil. |

### Anmärkningar

**Learn more**

* More details about policies: [Use of redaction policies](https://docs.groupdocs.com/redaction/net/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)

### Exempel

Följande exempel visar hur man tillämpar en redigeringspolicy på alla filer i en given inkommande mapp och sparar till en av de utgående mapparna – för framgångsrikt uppdaterade filer och för misslyckade.

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

Följande exempel innehåller en exempel‑XML‑policyfil med exempelkonfigurationer för alla typer av redigeringar.

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

### Se även

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
