---
title: Redactor
second_title: Riferimento API GroupDocs.Redaction per .NET
description: Rappresenta una classe principale che controlla il processo di redazione dei documenti consentendo di aprire redigere e salvare i documenti.
type: docs
weight: 650
url: /it/net/groupdocs.redaction/redactor/
---
## Redactor class

Rappresenta una classe principale che controlla il processo di redazione dei documenti, consentendo di aprire, redigere e salvare i documenti.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Inizializza una nuova istanza di[`Redactor`](../redactor) classe utilizzando stream. |
| [Redactor](redactor#constructor_3)(string) | Inizializza una nuova istanza di[`Redactor`](../redactor) classe utilizzando il percorso del file. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Inizializza una nuova istanza di[`Redactor`](../redactor) class per un documento protetto da password utilizzando stream. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Inizializza una nuova istanza di[`Redactor`](../redactor) class per un documento protetto da password utilizzando il suo percorso. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Inizializza una nuova istanza di[`Redactor`](../redactor) class per un documento protetto da password utilizzando stream e impostazioni. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Inizializza una nuova istanza di[`Redactor`](../redactor) class per un documento protetto da password utilizzando il percorso e le impostazioni. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Applica una redazione al documento. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Applica un criterio di redazione al documento. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Applica una serie di redazioni al documento. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Rilascia risorse. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Genera immagini di anteprima di pagine specifiche in un determinato formato immagine. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Recupera le informazioni generali sul documento: dimensioni, numero di pagine, ecc. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Salva il documento in un file con le seguenti opzioni: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Salva il documento in un file. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | Salva il documento in un flusso, inclusa la posizione personalizzata. |

### Osservazioni

**Scopri di più**

* Maggiori dettagli sull'applicazione delle redazioni: [Nozioni di base sulla redazione](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Argomenti di redazione più avanzati: [Utilizzo avanzato](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Esempi

L'esempio seguente mostra l'applicazione di una singola redazione al documento.

L'esempio seguente mostra l'applicazione di un elenco di redazioni al documento.

L'esempio seguente mostra come applicare un criterio di revisione a tutti i file all'interno di una determinata cartella in entrata e salvare in una delle cartelle in uscita, per i file aggiornati correttamente e per quelli non riusciti.

L'esempio seguente mostra come aprire un documento protetto da password utilizzando LoadOptions.

L'esempio seguente mostra come salvare un documento utilizzando SaveOptions.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   RedactorChangeLog result = redactor.Apply(new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")));
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   var redactionList = new Redaction[] 
   {
      new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
      new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(System.Drawing.Color.Red)),
      new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
      new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(System.Drawing.Color.Blue)),
      // ... altre redazioni
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // false, se almeno una redazione non è riuscita
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

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
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Qui possiamo usare l'istanza del documento per eseguire redazioni
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // La redazione del documento va qui
       //...
    
       // Salva il documento con le opzioni predefinite (converti le pagine in immagini, salva come PDF)
       redactor.Save();
    
       // Salva il documento nel formato originale sovrascrivendo il file originale
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Salva il documento nel file "*_Redacted.*" nel formato originale
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Salva il documento in "*_AnyText.*" (ad es. timestamp invece di "AnyText") nel suo nome file senza rasterizzazione
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Guarda anche

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* spazio dei nomi [GroupDocs.Redaction](../../groupdocs.redaction)
* assemblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
