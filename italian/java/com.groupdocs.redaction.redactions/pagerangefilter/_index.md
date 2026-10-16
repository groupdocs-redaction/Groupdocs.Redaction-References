---
title: "PageRangeFilter"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta il filtro di redazione che imposta l'intervallo di pagine all'interno di un documento per applicare la redazione."
type: docs
weight: 24
url: /it/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

Rappresenta un filtro di redazione, impostando l'intervallo di pagine all'interno di un documento per applicare la redazione.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | Inizializza una nuova istanza della classe RemovePageRedaction. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | Ottiene la posizione di riferimento di ricerca, l'inizio o la fine di un documento. |
|
|  | [getIndex()](#getIndex--) | Ottiene l'indice della posizione iniziale (basato su zero). |
|
|  | [getCount()](#getCount--) | Ottiene il conteggio delle pagine da rimuovere. |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | Verifica se questo intervallo di pagine del filtro contiene la pagina specificata. |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


Inizializza una nuova istanza della classe RemovePageRedaction.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | Posizione di riferimento di ricerca, l'inizio o la fine di un documento |
|
|  | indice | int | Indice della posizione iniziale (basato su zero) |
|
|  | conteggio | int | Numero di pagine da rimuovere |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


Ottiene la posizione di riferimento di ricerca, l'inizio o la fine di un documento.


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Ottiene l'indice della posizione iniziale (basato su zero).


**Returns:**
int - Indice di posizione iniziale (basato su zero).

### getCount() {#getCount--}
```
public final int getCount()
```


Ottiene il conteggio delle pagine da rimuovere.


**Returns:**
int - Il numero di pagine da rimuovere.

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


Verifica se questo intervallo di pagine del filtro contiene la pagina specificata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | indice della pagina (basato su zero) |
|
|  | pageCount | int | conteggio totale delle pagine |
|

**Returns:**
boolean - true, se questo intervallo di filtro contiene la pagina

