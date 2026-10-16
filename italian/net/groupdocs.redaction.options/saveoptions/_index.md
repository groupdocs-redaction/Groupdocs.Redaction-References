---
title: "SaveOptions"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Fornisce opzioni per modificare il nome del file di output e/o convertire il documento in rasterizzazione PDF basata su immagine."
type: docs
weight: 450
url: /it/net/groupdocs.redaction.options/saveoptions/
---
## SaveOptions class

Fornisce le opzioni per modificare il nome del file di output e/o convertire il documento in PDF basato su immagine (rasterizzazione).

```csharp
public class SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SaveOptions](saveoptions#constructor)() | Inizializza una nuova istanza con i valori predefiniti: rasterizzare in PDF - false, aggiungere suffisso - false. |
| [SaveOptions](saveoptions#constructor_1)(bool, string) | Inizializza una nuova istanza con i parametri forniti. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AddSuffix](../../groupdocs.redaction.options/saveoptions/addsuffix) { get; set; } | Ottiene o imposta un valore che indica se il nome file deve essere modificato prima del salvataggio. False per impostazione predefinita. |
| [Rasterization](../../groupdocs.redaction.options/saveoptions/rasterization) { get; } | Ottiene le impostazioni di rasterizzazione. |
| [RasterizeToPDF](../../groupdocs.redaction.options/saveoptions/rasterizetopdf) { get; set; } | Ottiene o imposta un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. |
| [RedactedFileSuffix](../../groupdocs.redaction.options/saveoptions/redactedfilesuffix) { get; set; } | Ottiene o imposta un suffisso personalizzato per il nome del file di output. Se non specificato, verrà usata la costante [`SaveSuffix`](./savesuffix). |
| [WordprocessingSaveOptions](../../groupdocs.redaction.options/saveoptions/wordprocessingsaveoptions) { get; } | Ottiene le opzioni di salvataggio specifiche per i documenti di elaborazione testi. |

## Campi

| Nome | Descrizione |
| --- | --- |
| const [SaveSuffix](../../groupdocs.redaction.options/saveoptions/savesuffix) | Rappresenta il valore predefinito del suffisso, che è "Redacted". |

### Osservazioni

**Learn more**

* [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
* [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
* [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
* [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

### Esempi

Il seguente esempio dimostra come salvare un documento usando SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // La redazione del documento va qui
       // ...
    
       // Salva il documento con le opzioni predefinite (converti le pagine in immagini, salva come PDF)
       redactor.Save();
    
       // Salva il documento nel formato originale sovrascrivendo il file originale
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Salva il documento nel file "*_Redacted.*" nel formato originale
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Salva il documento nel file "*_AnyText.*" (ad es. timestamp al posto di "AnyText") nel suo nome file senza rasterizzazione
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Vedi anche

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
