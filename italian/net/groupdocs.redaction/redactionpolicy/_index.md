---
title: RedactionPolicy
second_title: Riferimento API GroupDocs.Redaction per .NET
description: Rappresenta una politica di sanificazione contenente un insieme di redazioni specifiche da applicare.
type: docs
weight: 400
url: /it/net/groupdocs.redaction/redactionpolicy/
---
## RedactionPolicy class

Rappresenta una politica di sanificazione, contenente un insieme di redazioni specifiche da applicare.

```csharp
public class RedactionPolicy
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RedactionPolicy](redactionpolicy#constructor)() | Crea una nuova istanza del criterio Redazione. |
| [RedactionPolicy](redactionpolicy#constructor_1)(Redaction[]) | Crea una nuova istanza del criterio di redazione con un elenco specifico di redazioni. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Redactions](../../groupdocs.redaction/redactionpolicy/redactions) { get; } | Ottiene un array di file completamente configurati[`Redaction`](../redaction) -classi derivate. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load)(Stream) | Carica un'istanza di[`RedactionPolicy`](../redactionpolicy) da un flusso. |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load_1)(string) | Carica un'istanza di[`RedactionPolicy`](../redactionpolicy) da un percorso file. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save)(Stream) | Salva il criterio di redazione in un flusso. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save_1)(string) | Salva il criterio di redazione in un file. |

### Osservazioni

**Scopri di più**

* Ulteriori dettagli sulle norme: [Uso delle politiche redazionali](https://docs.groupdocs.com/redaction/net/use-redaction-policies/)
* Maggiori dettagli sull'applicazione delle redazioni: [Nozioni di base sulla redazione](https://docs.groupdocs.com/redaction/net/redaction-basics/)

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

* spazio dei nomi [GroupDocs.Redaction](../../groupdocs.redaction)
* assemblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->