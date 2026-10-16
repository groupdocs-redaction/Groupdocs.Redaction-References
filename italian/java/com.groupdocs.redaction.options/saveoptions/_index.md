---
title: "SaveOptions"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Fornisce opzioni per modificare il nome del file di output e/o convertire il documento in rasterizzazione PDF basata su immagine."
type: docs
weight: 14
url: /it/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

Fornisce opzioni per modificare il nome del file di output e/o convertire il documento in PDF basato su immagine (rasterizzazione).

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | Inizializza una nuova istanza con i valori predefiniti: rasterizza in PDF - false, aggiungi suffisso - false. |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | Inizializza una nuova istanza con i parametri forniti. |
|
## Campi

| Campo | Descrizione |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | Rappresenta il valore predefinito del suffisso, che è "Redacted". |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | Ottiene un valore che indica se il nome file deve essere modificato prima del salvataggio. |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | Imposta un valore che indica se il nome file deve essere modificato prima del salvataggio. |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | Ottiene un suffisso personalizzato per il nome file di output. |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | Imposta un suffisso personalizzato per il nome file di output. |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | Ottiene un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | Imposta un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. |
|
|  | [getRasterization()](#getRasterization--) | Ottiene le impostazioni di rasterizzazione. |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | Opzioni di salvataggio per l'elaborazione testi. |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


Inizializza una nuova istanza con i valori predefiniti: rasterizza in PDF - false, aggiungi suffisso - false.


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


Inizializza una nuova istanza con i parametri forniti.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | True, se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF |
|
|  | suffix | java.lang.String | Questo testo verrà aggiunto alla fine del nome file, se non è vuoto imposta anche AddSuffix su true |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


Rappresenta il valore predefinito del suffisso, che è "Redacted".


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


Ottiene un valore che indica se il nome file deve essere modificato prima del salvataggio. False per impostazione predefinita.


**Returns:**
boolean - Un valore che indica se il nome file deve essere modificato prima del salvataggio. False per impostazione predefinita.

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


Imposta un valore che indica se il nome file deve essere modificato prima del salvataggio. False per impostazione predefinita.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se il nome file deve essere modificato prima del salvataggio. False per impostazione predefinita. |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


Ottiene un suffisso personalizzato per il nome file di output. Se non è specificato, il
SaveSuffix
costante verrà utilizzata.


**Returns:**
java.lang.String - Un suffisso personalizzato per il nome file di output. Se non è specificato, la costante  SaveSuffix  verrà utilizzata.

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


Imposta un suffisso personalizzato per il nome file di output. Se non è specificato, il
SaveSuffix
costante verrà utilizzata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Un suffisso personalizzato per il nome del file di output. Se non è specificato, verrà usata la costante  SaveSuffix . |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


Ottiene un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF.


**Returns:**
boolean - Un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF.

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


Imposta un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


Ottiene le impostazioni di rasterizzazione.


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


Opzioni di salvataggio per l'elaborazione testi.


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
