---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt eine Redaktion dar, die ein farbiges Rechteck im angegebenen Bereich eines Bilddokuments platziert."
type: docs
weight: 18
url: /de/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

Stellt eine Redaktion dar, die ein farbiges Rechteck im angegebenen Bereich eines Bilddokuments platziert.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Initialisiert eine neue Instanz der Klasse ImageAreaRedaction zum Redigieren einer bestimmten Bereichsgröße. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getOptions()](#getOptions--) | Liest das |
RegionReplacementOptions
Optionen mit Farb- und Flächenparametern.
|
|  | [getTopLeft()](#getTopLeft--) | Gibt die obere linke Position des zu entfernenden Bereichs zurück |
|
|  | [getDescription()](#getDescription--) | Gibt eine Zeichenkette zurück, die die Redaktion und ihre Parameter beschreibt. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


Initialisiert eine neue Instanz der Klasse ImageAreaRedaction zum Redigieren einer bestimmten Bereichsgröße.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Koordinaten des Bereichs oben links |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Größe und Farbe des Bereichs |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


Liest das
RegionReplacementOptions
Optionen mit Farb- und Flächenparametern.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


Gibt die obere linke Position des zu entfernenden Bereichs zurück


**Returns:**
java.awt.Point - Die obere linke Position des zu entfernenden Bereichs

### getDescription() {#getDescription--}
```
public String getDescription()
```


Gibt eine Zeichenkette zurück, die die Redaktion und ihre Parameter beschreibt.


**Returns:**
java.lang.String - Text, der den Namen der Redaktion und Parameter enthält.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Wendet die Redaktion auf eine gegebene Formatinstanz an.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Eine Instanz eines Dokuments, auf das die Redaktion angewendet wird |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

