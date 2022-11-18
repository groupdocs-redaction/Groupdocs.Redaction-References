---
title: Load
second_title: GroupDocs.Redaction för .NET API-referens
description: Laddar en instans avRedactionPolicygroupdocs.redaction/redactionpolicy från en filsökväg.
type: docs
weight: 20
url: /sv/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

Laddar en instans av[`RedactionPolicy`](../../redactionpolicy) från en filsökväg.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Sökväg till XML-fil |

### Returvärde

Redaktionspolicy

### Exempel

Följande exempel visar hur man tillämpar en redigeringspolicy på alla filer i en given inkommande mapp och sparar i en av utgående mappar - för framgångsrikt uppdaterade filer och för misslyckade.

Följande exempel innehåller ett exempel på en XML-policyfil med exempelkonfigurationer för alla typer av redigeringar.

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

### Se även

* class [RedactionPolicy](../../redactionpolicy)
* namnutrymme [GroupDocs.Redaction](../../redactionpolicy)
* hopsättning [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

Laddar en instans av[`RedactionPolicy`](../../redactionpolicy) från en ström.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| input | Stream | Ström som innehåller XML-konfiguration |

### Returvärde

Redaktionspolicy

### Exempel

Följande exempel visar hur man tillämpar en redigeringspolicy på alla filer i en given inkommande mapp och sparar i en av utgående mappar - för framgångsrikt uppdaterade filer och för misslyckade.

Följande exempel innehåller ett exempel på en XML-policyfil med exempelkonfigurationer för alla typer av redigeringar.

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

### Se även

* class [RedactionPolicy](../../redactionpolicy)
* namnutrymme [GroupDocs.Redaction](../../redactionpolicy)
* hopsättning [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
