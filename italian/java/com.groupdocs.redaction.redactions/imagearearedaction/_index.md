---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta una redazione che inserisce un rettangolo colorato nell'area specificata di un documento immagine."
type: docs
weight: 18
url: /it/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

Rappresenta una redazione che inserisce un rettangolo colorato nell'area specificata di un documento immagine.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Inizializza una nuova istanza della classe ImageAreaRedaction per la redazione di un'area di dimensioni specifiche. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getOptions()](#getOptions--) | Ottiene il |
RegionReplacementOptions
opzioni con parametri di colore e area.
|
|  | [getTopLeft()](#getTopLeft--) | Ottiene la posizione in alto a sinistra dell'area da rimuovere |
|
|  | [getDescription()](#getDescription--) | Restituisce una stringa che descrive la redazione e i suoi parametri. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applica la redazione a una determinata istanza di formato. |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


Inizializza una nuova istanza della classe ImageAreaRedaction per la redazione di un'area di dimensioni specifiche.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Coordinate dell'area in alto a sinistra |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Dimensione e colore dell'area |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


Ottiene il
RegionReplacementOptions
opzioni con parametri di colore e area.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


Ottiene la posizione in alto a sinistra dell'area da rimuovere


**Returns:**
java.awt.Point - La posizione in alto a sinistra dell'area da rimuovere

### getDescription() {#getDescription--}
```
public String getDescription()
```


Restituisce una stringa che descrive la redazione e i suoi parametri.


**Returns:**
java.lang.String - Testo, contenente il nome della redazione e i parametri.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applica la redazione a una determinata istanza di formato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Un'istanza di un documento a cui applicare la redazione |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

