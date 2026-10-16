---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta i parametri di colore e area per la sostituzione di una regione immagine."
type: docs
weight: 29
url: /it/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

Rappresenta i parametri di colore e area per la sostituzione di regioni immagine. Vedi
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | Inizializza una nuova istanza della classe RegionReplacementOptions. |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | Inizializza una nuova istanza della classe RegionReplacementOptions la cui dimensione corrisponde al testo fornito. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | Restituisce il colore per riempire l'area redatta. |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | Imposta il colore per riempire l'area redatta. |
|
|  | [getSize()](#getSize--) | Ottiene il rettangolo con larghezza e altezza. |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | Imposta il rettangolo con larghezza e altezza. |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


Inizializza una nuova istanza della classe RegionReplacementOptions.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Colore per riempire l'area |
|
|  | size | java.awt.Dimension | Dimensione dell'area riempita |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


Inizializza una nuova istanza della classe RegionReplacementOptions la cui dimensione corrisponde al testo fornito.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Colore per riempire l'area |
|
|  | font | java.awt.Font | Font del testo previsto |
|
|  | expectedText | java.lang.String | Testo previsto |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


Restituisce il colore per riempire l'area redatta.


**Returns:**
java.awt.Color - Il colore per riempire l'area redatta.

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


Imposta il colore per riempire l'area redatta.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.awt.Color | Il colore per riempire l'area redatta. |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


Ottiene il rettangolo con larghezza e altezza.


**Returns:**
java.awt.Dimension - Il rettangolo con larghezza e altezza.

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


Imposta il rettangolo con larghezza e altezza.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.awt.Dimension | Il rettangolo con larghezza e altezza. |
|

