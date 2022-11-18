---
title: Load
second_title: Riferimento API GroupDocs.Redaction per .NET
description: Carica unistanza diRedactionPolicygroupdocs.redaction/redactionpolicy da un percorso file.
type: docs
weight: 20
url: /it/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

Carica un'istanza di[`RedactionPolicy`](../../redactionpolicy) da un percorso file.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Percorso del file XML |

### Valore di ritorno

Politica di redazione

### Esempi

L'esempio seguente mostra come applicare un criterio di revisione a tutti i file all'interno di una determinata cartella in entrata e salvare in una delle cartelle in uscita, per i file aggiornati correttamente e per quelli non riusciti.

L'esempio seguente contiene un file di criteri XML di esempio con configurazioni di esempio per tutti i tipi di redazioni.

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

### Guarda anche

* class [RedactionPolicy](../../redactionpolicy)
* spazio dei nomi [GroupDocs.Redaction](../../redactionpolicy)
* assemblea [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

Carica un'istanza di[`RedactionPolicy`](../../redactionpolicy) da un flusso.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| input | Stream | Stream contenente la configurazione XML |

### Valore di ritorno

Politica di redazione

### Esempi

L'esempio seguente mostra come applicare un criterio di revisione a tutti i file all'interno di una determinata cartella in entrata e salvare in una delle cartelle in uscita, per i file aggiornati correttamente e per quelli non riusciti.

L'esempio seguente contiene un file di criteri XML di esempio con configurazioni di esempio per tutti i tipi di redazioni.

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

### Guarda anche

* class [RedactionPolicy](../../redactionpolicy)
* spazio dei nomi [GroupDocs.Redaction](../../redactionpolicy)
* assemblea [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
