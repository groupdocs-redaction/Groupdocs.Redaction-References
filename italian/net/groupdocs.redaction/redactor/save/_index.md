---
title: "Salva"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Salva il documento in un file con le seguenti opzioni AddSuffix  true RasterizeToPDF  true."
type: docs
weight: 60
url: /it/net/groupdocs.redaction/redactor/save/
---
## Save() {#save}

Salva il documento in un file con le seguenti opzioni: AddSuffix = true, RasterizeToPDF = true.

```csharp
public string Save()
```

### Valore di ritorno

Percorso del documento redatto

### Vedi anche

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Save(SaveOptions) {#save_1}

Salva il documento in un file.

```csharp
public string Save(SaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveOptions | SaveOptions | Opzioni per aggiungere il suffisso o rasterizzare |

### Valore di ritorno

Percorso del documento redatto

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

* class [SaveOptions](../../../groupdocs.redaction.options/saveoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Save(Stream, SaveOptions) {#save_3}

Salva il documento nello stream specificato.

```csharp
public void Save(Stream document, SaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| documento | Stream | Il flusso di destinazione. |
| saveOptions | SaveOptions | Le opzioni di salvataggio che controllano la rasterizzazione, il suffisso del nome file di output e le impostazioni di salvataggio specifiche per il documento. |

### Vedi anche

* class [SaveOptions](../../../groupdocs.redaction.options/saveoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
