---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Fornisce opzioni per impostare i requisiti e i delegati di stream per la generazione dell'anteprima."
type: docs
weight: 11
url: /it/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Fornisce opzioni per impostare i requisiti e i delegati di stream per la generazione dell'anteprima.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | Inizializza una nuova istanza della classe PreviewOptions, causando la chiusura del flusso di output. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Inizializza una nuova istanza della classe PreviewOptions, facendo restituire il flusso di output al client per un ulteriore utilizzo. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getWidth()](#getWidth--) | Ottiene o imposta la larghezza dell'anteprima della pagina. |
|
|  | [setWidth(int value)](#setWidth-int-) | Ottiene o imposta la larghezza dell'anteprima della pagina. |
|
|  | [getHeight()](#getHeight--) | Ottiene o imposta l'altezza dell'anteprima della pagina. |
|
|  | [setHeight(int value)](#setHeight-int-) | Ottiene o imposta l'altezza dell'anteprima della pagina. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Ottiene o imposta un array di numeri di pagina per generare l'anteprima. |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | Ottiene o imposta un array di numeri di pagina per generare l'anteprima. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Ottiene o imposta il formato dell'immagine di anteprima. |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | Ottiene o imposta il formato dell'immagine di anteprima. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Ottiene o imposta un'istanza del delegato di creazione dello stream della pagina. |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | Ottiene o imposta un'istanza del delegato di creazione dello stream della pagina. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Ottiene o imposta un'istanza del delegato di completamento dell'anteprima della pagina. |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Ottiene o imposta un'istanza del delegato di completamento dell'anteprima della pagina. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Inizializza una nuova istanza della classe PreviewOptions, causando la chiusura del flusso di output.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Crea uno stream per una specifica anteprima di pagina |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Inizializza una nuova istanza della classe PreviewOptions, facendo restituire il flusso di output al client per un ulteriore utilizzo.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Crea uno stream per una specifica anteprima di pagina |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Notifica che la generazione dell'anteprima della pagina è completata e ottiene lo stream di output |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


Ottiene o imposta la larghezza dell'anteprima della pagina.


**Returns:**
int - Larghezza dell'anteprima della pagina.

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


Ottiene o imposta la larghezza dell'anteprima della pagina.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Larghezza dell'anteprima della pagina. |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


Ottiene o imposta l'altezza dell'anteprima della pagina.


**Returns:**
int - Altezza dell'anteprima della pagina.

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


Ottiene o imposta l'altezza dell'anteprima della pagina.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Altezza dell'anteprima della pagina. |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


Ottiene o imposta un array di numeri di pagina per generare l'anteprima.


**Returns:**
int[] - Un array di numeri di pagina per generare l'anteprima.

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


Ottiene o imposta un array di numeri di pagina per generare l'anteprima.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int[] | Un array di numeri di pagina per generare l'anteprima. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


Ottiene o imposta il formato dell'immagine di anteprima.


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


Ottiene o imposta il formato dell'immagine di anteprima.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | Formato dell'immagine di anteprima. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


Ottiene o imposta un'istanza del delegato di creazione dello stream della pagina.


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


Ottiene o imposta un'istanza del delegato di creazione dello stream della pagina.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Un'istanza del delegato di creazione dello stream della pagina. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


Ottiene o imposta un'istanza del delegato di completamento dell'anteprima della pagina.


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


Ottiene o imposta un'istanza del delegato di completamento dell'anteprima della pagina.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Un'istanza del delegato di completamento dell'anteprima della pagina. |
|

