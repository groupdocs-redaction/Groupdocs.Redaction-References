---
title: "Redactor"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta la classe principale che controlla il processo di redazione dei documenti, consentendo di aprire, redigere e salvare i documenti."
type: docs
weight: 16
url: /it/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

Rappresenta la classe principale che controlla il processo di redazione dei documenti, consentendo di aprire, redigere e salvare i documenti.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | Inizializza una nuova istanza di |
Redactor
classe utilizzando il percorso del file.
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | Inizializza una nuova istanza di |
Redactor
classe utilizzando lo stream.
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | Inizializza una nuova istanza di |
Redactor
classe per un documento protetto da password utilizzando il suo percorso.
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Inizializza una nuova istanza di |
Redactor
classe per un documento protetto da password utilizzando il suo percorso e le impostazioni.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | Inizializza una nuova istanza di |
Redactor
classe per un documento protetto da password utilizzando lo stream.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Inizializza una nuova istanza di |
Redactor
classe per un documento protetto da password utilizzando lo stream e le impostazioni.
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [close()](#close--) | Rilascia le risorse. |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | Applica una redazione al documento. |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | Applica un insieme di redazioni al documento. |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | Applica una politica di redazione al documento. |
|
|  | [save()](#save--) | Salva il documento su un file con le seguenti opzioni: AddSuffix = true, RasterizeToPDF = true. |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | Salva il documento su un file. |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | Salva il documento su uno stream. |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | Salva il documento su uno stream. |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | Salva il documento su uno stream, includendo una posizione personalizzata. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | Genera immagini di anteprima di pagine specifiche in un formato immagine specificato. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Ottiene le informazioni generali sul documento - dimensione, numero di pagine, ecc. |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


Inizializza una nuova istanza di
Redactor
classe utilizzando il percorso del file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Percorso del file |


Il seguente esempio dimostra come aprire un documento per la redazione.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
     // Here we can use document instance to perform redactions
 }
 
``` 
````

 |

### Redactor(InputStream document) {#Redactor-java.io.InputStream-}
```
public Redactor(InputStream document)
```


Initializes a new instance of 
Redactor
 class using stream.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source stream of the document


The following example demonstrates how to open a document from stream.

````

try (InputStream stream = new FileInputStream("C:\\sample.pdf"))
{
try (Redactor redactor = new Redactor(stream))
{
// Qui possiamo usare l'istanza del documento per eseguire le redazioni
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


Inizializza una nuova istanza di
Redactor
classe per un documento protetto da password utilizzando il suo percorso.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Percorso al file. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opzioni, inclusa la password. |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


Inizializza una nuova istanza di
Redactor
classe per un documento protetto da password utilizzando il suo percorso e le impostazioni.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Percorso al file. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opzioni dipendenti dal file, inclusa la password. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Impostazioni predefinite per il processo di redazione. |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


Inizializza una nuova istanza di
Redactor
classe per un documento protetto da password utilizzando lo stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documento | java.io.InputStream | Flusso di input di origine. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opzioni, inclusa la password. |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


Inizializza una nuova istanza di
Redactor
classe per un documento protetto da password utilizzando lo stream e le impostazioni.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documento | java.io.InputStream | Flusso di input di origine. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opzioni, inclusa la password. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Impostazioni predefinite per il processo di redazione. |
|

### close() {#close--}
```
public final void close()
```


Rilascia le risorse.


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


Applica una redazione al documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Un'istanza di Redaction da applicare |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


Applica un insieme di redazioni al documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Un array di redazioni da applicare |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


Applica una politica di redazione al documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | Politica di redazione |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


Salva il documento su un file con le seguenti opzioni: AddSuffix = true, RasterizeToPDF = true.


**Returns:**
java.lang.String - Percorso del documento redatto

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


Salva il documento su un file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Opzioni per aggiungere un suffisso o rasterizzare |
|

**Returns:**
java.lang.String - Percorso del documento redatto

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


Salva il documento su uno stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documento | java.io.OutputStream | Flusso di destinazione |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


Salva il documento su uno stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documento | java.io.OutputStream | Flusso di destinazione |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Opzioni di salvataggio |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


Salva il documento su uno stream, includendo una posizione personalizzata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documento | java.io.OutputStream | Flusso di destinazione |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | Opzioni per rasterizzare o meno e per specificare le pagine da rasterizzare |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


Genera immagini di anteprima di pagine specifiche in un formato immagine specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | Impostazioni delle proprietà dell'immagine e dell'intervallo di pagine |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


Ottiene le informazioni generali sul documento - dimensione, numero di pagine, ecc.


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

