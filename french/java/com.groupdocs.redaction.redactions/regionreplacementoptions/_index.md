---
title: "RegionReplacementOptions"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente les paramètres de couleur et de zone pour le remplacement d'une région d'image."
type: docs
weight: 29
url: /fr/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

Représente les paramètres de couleur et de zone pour le remplacement de région d'image. Voir
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | Initialise une nouvelle instance de la classe RegionReplacementOptions. |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | Initialise une nouvelle instance de la classe RegionReplacementOptions dont la taille correspond au texte donné. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | Obtient la couleur pour remplir la zone rédigée. |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | Définit la couleur pour remplir la zone rédigée. |
|
|  | [getSize()](#getSize--) | Obtient le rectangle avec largeur et hauteur. |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | Définit le rectangle avec largeur et hauteur. |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


Initialise une nouvelle instance de la classe RegionReplacementOptions.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Couleur pour remplir la zone |
|
|  | taille | java.awt.Dimension | Taille de la zone remplie |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


Initialise une nouvelle instance de la classe RegionReplacementOptions dont la taille correspond au texte donné.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Couleur pour remplir la zone |
|
|  | font | java.awt.Font | Police du texte attendu |
|
|  | expectedText | java.lang.String | Texte attendu |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


Obtient la couleur pour remplir la zone rédigée.


**Returns:**
java.awt.Color - La couleur pour remplir la zone censurée.

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


Définit la couleur pour remplir la zone rédigée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.awt.Color | La couleur pour remplir la zone censurée. |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


Obtient le rectangle avec largeur et hauteur.


**Returns:**
java.awt.Dimension - Le rectangle avec largeur et hauteur.

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


Définit le rectangle avec largeur et hauteur.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.awt.Dimension | Le rectangle avec largeur et hauteur. |
|

