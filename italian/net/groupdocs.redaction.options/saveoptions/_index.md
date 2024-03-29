---
title: SaveOptions
second_title: Riferimento API GroupDocs.Redaction per .NET
description: Fornisce opzioni per modificare il nome di un file di output e/o convertire il documento in PDF basato su immagini rasterizzazione.
type: docs
weight: 380
url: /it/net/groupdocs.redaction.options/saveoptions/
---
## SaveOptions class

Fornisce opzioni per modificare il nome di un file di output e/o convertire il documento in PDF basato su immagini (rasterizzazione).

```csharp
public class SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SaveOptions](saveoptions#constructor)() | Inizializza una nuova istanza con impostazioni predefinite: rasterizza in PDF - false, aggiungi suffisso - false. |
| [SaveOptions](saveoptions#constructor_1)(bool, string) | Inizializza una nuova istanza con determinati parametri. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AddSuffix](../../groupdocs.redaction.options/saveoptions/addsuffix) { get; set; } | Ottiene o imposta un valore che indica se il nome del file deve essere modificato prima del salvataggio. Falso per impostazione predefinita. |
| [Rasterization](../../groupdocs.redaction.options/saveoptions/rasterization) { get; } | Ottiene le impostazioni di rasterizzazione. |
| [RasterizeToPDF](../../groupdocs.redaction.options/saveoptions/rasterizetopdf) { get; set; } | Ottiene o imposta un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un singolo file PDF. |
| [RedactedFileSuffix](../../groupdocs.redaction.options/saveoptions/redactedfilesuffix) { get; set; } | Ottiene o imposta un suffisso personalizzato per il nome del file di output. Se non è specificato, il[`SaveSuffix`](./savesuffix) verrà utilizzata la costante. |

## Campi

| Nome | Descrizione |
| --- | --- |
| const [SaveSuffix](../../groupdocs.redaction.options/saveoptions/savesuffix) | Rappresenta il valore del suffisso predefinito, che è "Redacted". |

### Osservazioni

**Saperne di più**

* [Salva con le opzioni predefinite](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
* [Salva in PDF rasterizzato](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* [Seleziona pagine specifiche per PDF rasterizzati](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
* [Salva nel formato originale](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
* [Salva sovrascrivendo il file originale](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
* [Salva in streaming](https://docs.groupdocs.com/redaction/net/save-to-stream/)

### Esempi

L'esempio seguente mostra come salvare un documento utilizzando SaveOptions.

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

* spazio dei nomi [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assemblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
