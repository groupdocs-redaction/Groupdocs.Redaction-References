---
title: "PageAreaFilter"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta un filtro di redazione che imposta un'area all'interno di una pagina di un documento per applicare la redazione."
type: docs
weight: 22
url: /it/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

Rappresenta un filtro di redazione, impostando un'area all'interno di una pagina di un documento per applicare la redazione.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | Inizializza una nuova istanza della classe PageAreaFilter per redigere un'area specifica. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Restituisce il rettangolo (posizione in alto a sinistra e dimensione dell'area) su una pagina. |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | Verifica se quest'area del filtro ha intersezione con il rettangolo fornito. |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


Inizializza una nuova istanza della classe PageAreaFilter per redigere un'area specifica.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Coordinate dell'area in alto a sinistra |
|
|  | size | java.awt.Dimension | Dimensione e colore dell'area |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Restituisce il rettangolo (posizione in alto a sinistra e dimensione dell'area) su una pagina.


**Returns:**
java.awt.Rectangle - Il rettangolo (posizione in alto a sinistra e dimensione dell'area) su una pagina.

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


Verifica se quest'area del filtro ha intersezione con il rettangolo fornito.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | java.awt.Rectangle | Rettangolo da verificare |
|

**Returns:**
boolean - true, se quest'area del filtro ha intersezione

