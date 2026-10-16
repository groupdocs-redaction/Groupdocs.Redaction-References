---
title: "RedactionPolicy"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una politica di sanificazione contenente un insieme di redazioni specifiche da applicare."
type: docs
weight: 500
url: /it/net/groupdocs.redaction/redactionpolicy/
---
## RedactionPolicy class

Rappresenta una politica di sanitizzazione, contenente un insieme di redazioni specifiche da applicare.

```csharp
public class RedactionPolicy
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RedactionPolicy](redactionpolicy#constructor)() | Crea una nuova istanza della politica di redazione. |
| [RedactionPolicy](redactionpolicy#constructor_1)(Redaction[]) | Crea una nuova istanza della politica di redazione con un elenco specifico di redazioni. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Redactions](../../groupdocs.redaction/redactionpolicy/redactions) { get; } | Ottiene un array di classi derivate da [`Redaction`](../redaction). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load)(Stream) | Carica un'istanza di [`RedactionPolicy`](../redactionpolicy) da un flusso. |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load_1)(string) | Carica un'istanza di [`RedactionPolicy`](../redactionpolicy) da un percorso file. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save)(Stream) | Salva la politica di redazione su un flusso. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save_1)(string) | Salva la politica di redazione su un file. |

### Osservazioni

**Learn more**

* More details about policies: [Use of redaction policies](https://docs.groupdocs.com/redaction/net/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)

### Esempi

Il seguente esempio dimostra come applicare una politica di redazione a tutti i file all'interno di una cartella di ingresso specificata e salvarli in una delle cartelle di uscita — per i file aggiornati con successo e per quelli falliti.

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

Il seguente esempio contiene un file di politica XML di esempio con configurazioni di esempio per tutti i tipi di redazioni.

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

### Vedi anche

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
