---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Fornisce opzioni per convertire i file in PDF."
type: docs
weight: 12
url: /it/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

Fornisce opzioni per convertire i file in PDF.

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | Inizializza una nuova istanza. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Ottiene un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Imposta un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. |
|
|  | [getPageIndex()](#getPageIndex--) | Ottiene l'indice della prima pagina (basato su zero) da convertire in PDF. |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | Imposta l'indice della prima pagina (basato su zero) da convertire in PDF. |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | Ottiene un valore che indica se la proprietà PageIndex è stata modificata (impostata) dopo la sua inizializzazione. |
|
|  | [getPageCount()](#getPageCount--) | Ottiene il numero di pagine da convertire in PDF. |
|
|  | [setPageCount(int value)](#setPageCount-int-) | Imposta il numero di pagine da convertire in PDF. |
|
|  | [isPageCountSet()](#isPageCountSet--) | Ottiene un valore che indica se la proprietà PageCount è stata modificata (impostata) dopo la sua inizializzazione. |
|
|  | [getCompliance()](#getCompliance--) | Ottiene il livello di conformità PDF. |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | Imposta il livello di conformità PDF. |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | Ottiene un indicatore, che è vero se le opzioni avanzate di rasterizzazione sono impostate. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | È possibile utilizzare questo metodo per registrare un'opzione avanzata di rasterizzazione da applicare. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | È possibile utilizzare questo metodo per registrare un'opzione avanzata di rasterizzazione da applicare. |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


Inizializza una nuova istanza.


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


Ottiene un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. TRUE per impostazione predefinita, impostare a FALSE per evitare la rasterizzazione.


**Returns:**
boolean - Un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. TRUE per impostazione predefinita, impostare a FALSE per evitare la rasterizzazione.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


Imposta un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. TRUE per impostazione predefinita, impostare a FALSE per evitare la rasterizzazione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. TRUE per impostazione predefinita, impostare a FALSE per evitare la rasterizzazione. |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Ottiene l'indice della prima pagina (basato su zero) da convertire in PDF.


**Returns:**
int - L'indice della prima pagina (basato su 0) da convertire in PDF.

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Imposta l'indice della prima pagina (basato su zero) da convertire in PDF.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | L'indice della prima pagina (basato su 0) da convertire in PDF. |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


Ottiene un valore che indica se la proprietà PageIndex è stata modificata (impostata) dopo la sua inizializzazione.


**Returns:**
boolean - Un valore che indica se la proprietà PageIndex è stata modificata (impostata) dopo la sua inizializzazione.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Ottiene il numero di pagine da convertire in PDF.


**Returns:**
int - Il numero di pagine da convertire in PDF.

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Imposta il numero di pagine da convertire in PDF.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero di pagine da convertire in PDF. |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


Ottiene un valore che indica se la proprietà PageCount è stata modificata (impostata) dopo la sua inizializzazione.


**Returns:**
boolean - Un valore che indica se la proprietà PageCount è stata modificata (impostata) dopo la sua inizializzazione.

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


Ottiene il livello di conformità PDF.


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


Imposta il livello di conformità PDF.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | Il livello di conformità PDF. |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


Ottiene un indicatore, che è vero se le opzioni avanzate di rasterizzazione sono impostate.


**Returns:**
boolean - Un indicatore, che è vero se le opzioni avanzate di rasterizzazione sono impostate.

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


È possibile utilizzare questo metodo per registrare un'opzione avanzata di rasterizzazione da applicare.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Fornisce informazioni sul tipo di effetto selezionato (scala di grigi, bordo, ecc.) |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


È possibile utilizzare questo metodo per registrare un'opzione avanzata di rasterizzazione da applicare.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Fornisce informazioni sul tipo di effetto selezionato (scala di grigi, bordo, ecc.) |
|
|  | parametri | java.util.HashMap<java.lang.String,java.lang.String> | Parametri per l'effetto specificato, come l'angolo di rotazione |
|

