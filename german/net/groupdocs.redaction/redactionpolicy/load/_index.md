---
title: Load
second_title: GroupDocs.Redaction für .NET-API-Referenz
description: Lädt eine Instanz vonRedactionPolicygroupdocs.redaction/redactionpolicy aus einem Dateipfad.
type: docs
weight: 20
url: /de/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

Lädt eine Instanz von[`RedactionPolicy`](../../redactionpolicy) aus einem Dateipfad.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Pfad zur XML-Datei |

### Rückgabewert

Schwärzungsrichtlinie

### Beispiele

Das folgende Beispiel zeigt, wie eine Schwärzungsrichtlinie auf alle Dateien in einem bestimmten Eingangsordner angewendet und in einem der Ausgangsordner gespeichert wird – für erfolgreich aktualisierte Dateien und für fehlgeschlagene Dateien.

Das folgende Beispiel enthält eine Beispiel-XML-Richtliniendatei mit Beispielkonfigurationen für alle Schwärzungstypen.

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

### Siehe auch

* class [RedactionPolicy](../../redactionpolicy)
* namensraum [GroupDocs.Redaction](../../redactionpolicy)
* Montage [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

Lädt eine Instanz von[`RedactionPolicy`](../../redactionpolicy) aus einem Stream.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| input | Stream | Stream mit XML-Konfiguration |

### Rückgabewert

Schwärzungsrichtlinie

### Beispiele

Das folgende Beispiel zeigt, wie eine Schwärzungsrichtlinie auf alle Dateien in einem bestimmten Eingangsordner angewendet und in einem der Ausgangsordner gespeichert wird – für erfolgreich aktualisierte Dateien und für fehlgeschlagene Dateien.

Das folgende Beispiel enthält eine Beispiel-XML-Richtliniendatei mit Beispielkonfigurationen für alle Schwärzungstypen.

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

### Siehe auch

* class [RedactionPolicy](../../redactionpolicy)
* namensraum [GroupDocs.Redaction](../../redactionpolicy)
* Montage [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
