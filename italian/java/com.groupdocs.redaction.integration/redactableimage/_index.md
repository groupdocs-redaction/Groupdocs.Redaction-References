---
title: "RedactableImage"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Fornisce una facciata per tutte le operazioni di redazione di immagini raster."
type: docs
weight: 14
url: /it/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

Fornisce una facciata per tutte le operazioni di redazione di immagini raster.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | Crea una nuova istanza utilizzando un oggetto, implementando |
IImageFormatInstance
interfaccia.
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | Crea una nuova istanza utilizzando un oggetto, implementando |
IMultipleAreaRedactable
interfaccia.
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | Recupera uno stream con il contenuto reale dell'immagine. |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Oscura più aree dell'immagine contemporaneamente con lo stesso colore. |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Sostituisce l'area in un punto dato con un rettangolo di colore e dimensione specifici. |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


Crea una nuova istanza utilizzando un oggetto, implementando
IImageFormatInstance
interfaccia.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | Un'istanza, che implementa l'interfaccia IImageFormatInstance |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


Crea una nuova istanza utilizzando un oggetto, implementando
IMultipleAreaRedactable
interfaccia.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | Un'istanza, che implementa l'interfaccia IMultipleAreaRedactable |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


Recupera uno stream con il contenuto reale dell'immagine.


**Returns:**
java.io.InputStream - Stream, contenente dati dell'immagine

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


Oscura più aree dell'immagine contemporaneamente con lo stesso colore.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rettangoli | java.awt.Rectangle[] | Un array di aree rettangolari |
|
|  | boxColor | java.awt.Color | Colore per riempire le aree |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Sostituisce l'area in un punto dato con un rettangolo di colore e dimensione specifici.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Coordinate dell'angolo superiore sinistro dell'area riempita |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Impostazioni di colore e dimensione |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

