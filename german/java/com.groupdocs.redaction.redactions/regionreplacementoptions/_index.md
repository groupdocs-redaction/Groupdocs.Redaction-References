---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Farb- und Bereichsparameter für den Austausch von Bildregionen dar."
type: docs
weight: 29
url: /de/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

Stellt Farb‑ und Flächenparameter für den Bildbereichsaustausch dar. Siehe
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | Initialisiert eine neue Instanz der Klasse RegionReplacementOptions. |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | Initialisiert eine neue Instanz der Klasse RegionReplacementOptions, deren Größe dem angegebenen Text entspricht. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | Liefert die Farbe, mit der der redigierte Bereich gefüllt wird. |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | Setzt die Farbe, mit der der redigierte Bereich gefüllt wird. |
|
|  | [getSize()](#getSize--) | Liefert das Rechteck mit Breite und Höhe. |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | Setzt das Rechteck mit Breite und Höhe. |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


Initialisiert eine neue Instanz der Klasse RegionReplacementOptions.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Farbe zum Füllen des Bereichs |
|
|  | size | java.awt.Dimension | Größe des gefüllten Bereichs |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


Initialisiert eine neue Instanz der Klasse RegionReplacementOptions, deren Größe dem angegebenen Text entspricht.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Farbe zum Füllen des Bereichs |
|
|  | font | java.awt.Font | Erwartete Textschriftart |
|
|  | expectedText | java.lang.String | Erwarteter Text |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


Liefert die Farbe, mit der der redigierte Bereich gefüllt wird.


**Returns:**
java.awt.Color - Die Farbe, mit der der redigierte Bereich gefüllt wird.

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


Setzt die Farbe, mit der der redigierte Bereich gefüllt wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.awt.Color | Die Farbe, mit der der redigierte Bereich gefüllt wird. |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


Liefert das Rechteck mit Breite und Höhe.


**Returns:**
java.awt.Dimension - Das Rechteck mit Breite und Höhe.

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


Setzt das Rechteck mit Breite und Höhe.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.awt.Dimension | Das Rechteck mit Breite und Höhe. |
|

