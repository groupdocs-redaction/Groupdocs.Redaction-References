---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar färg- och områdesparametrar för ersättning av bildregion."
type: docs
weight: 29
url: /sv/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

Representerar färg‑ och områdesparametrar för ersättning av bildregion. Se
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | Initierar en ny instans av klassen RegionReplacementOptions. |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | Initierar en ny instans av klassen RegionReplacementOptions vars storlek matchar den givna texten. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | Hämtar färgen för att fylla det redigerade området. |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | Ställer in färgen för att fylla det redigerade området. |
|
|  | [getSize()](#getSize--) | Hämtar rektangeln med bredd och höjd. |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | Ställer in rektangeln med bredd och höjd. |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


Initierar en ny instans av klassen RegionReplacementOptions.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Färg för att fylla området |
|
|  | storlek | java.awt.Dimension | Storlek på fyllt område |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


Initierar en ny instans av klassen RegionReplacementOptions vars storlek matchar den givna texten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Färg för att fylla området |
|
|  | font | java.awt.Font | Förväntat texttypsnitt |
|
|  | expectedText | java.lang.String | Förväntad text |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


Hämtar färgen för att fylla det redigerade området.


**Returns:**
java.awt.Color - Färgen för att fylla det redigerade området.

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


Ställer in färgen för att fylla det redigerade området.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.awt.Color | Färgen för att fylla det redigerade området. |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


Hämtar rektangeln med bredd och höjd.


**Returns:**
java.awt.Dimension - Rektangeln med bredd och höjd.

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


Ställer in rektangeln med bredd och höjd.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.awt.Dimension | Rektangeln med bredd och höjd. |
|

