---
title: "ImageAreaRedaction"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente une rédaction qui place un rectangle coloré dans une zone donnée d'un document image."
type: docs
weight: 18
url: /fr/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

Représente une rédaction qui place un rectangle coloré dans une zone donnée d'un document image.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Initialise une nouvelle instance de la classe ImageAreaRedaction pour masquer une zone de taille spécifique. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getOptions()](#getOptions--) | Obtient le |
RegionReplacementOptions
options avec des paramètres de couleur et de zone.
|
|  | [getTopLeft()](#getTopLeft--) | Obtient la position en haut à gauche de la zone à supprimer |
|
|  | [getDescription()](#getDescription--) | Renvoie une chaîne, décrivant la rédaction et ses paramètres. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applique la rédaction à une instance de format donnée. |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


Initialise une nouvelle instance de la classe ImageAreaRedaction pour masquer une zone de taille spécifique.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Coordonnées de la zone en haut à gauche |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Taille et couleur de la zone |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


Obtient le
RegionReplacementOptions
options avec des paramètres de couleur et de zone.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


Obtient la position en haut à gauche de la zone à supprimer


**Returns:**
java.awt.Point - La position en haut à gauche de la zone à supprimer

### getDescription() {#getDescription--}
```
public String getDescription()
```


Renvoie une chaîne, décrivant la rédaction et ses paramètres.


**Returns:**
java.lang.String - Texte contenant le nom de la rédaction et les paramètres.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applique la rédaction à une instance de format donnée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Une instance d'un document pour appliquer la rédaction |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

