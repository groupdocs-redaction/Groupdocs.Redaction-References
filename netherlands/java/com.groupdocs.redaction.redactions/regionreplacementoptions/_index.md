---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Vertegenwoordigt kleur- en gebiedsparameters voor het vervangen van een afbeeldingsgebied."
type: docs
weight: 29
url: /nl/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

Stelt kleur‑ en gebiedsparameters voor vervanging van afbeeldingsgebieden voor. Zie
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | Initialiseert een nieuw exemplaar van de klasse RegionReplacementOptions. |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | Initialiseert een nieuw exemplaar van de klasse RegionReplacementOptions waarvan de grootte overeenkomt met de opgegeven tekst. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | Haalt de kleur op om het geredigeerde gebied te vullen. |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | Stelt de kleur in om het geredigeerde gebied te vullen. |
|
|  | [getSize()](#getSize--) | Haalt de rechthoek met en hoogte op. |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | Stelt de rechthoek met en hoogte in. |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


Initialiseert een nieuw exemplaar van de klasse RegionReplacementOptions.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Kleur om het gebied te vullen |
|
|  | size | java.awt.Dimension | Grootte van het gevulde gebied |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


Initialiseert een nieuw exemplaar van de klasse RegionReplacementOptions waarvan de grootte overeenkomt met de opgegeven tekst.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Kleur om het gebied te vullen |
|
|  | font | java.awt.Font | Verwacht lettertype van de tekst |
|
|  | expectedText | java.lang.String | Verwachte tekst |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


Haalt de kleur op om het geredigeerde gebied te vullen.


**Returns:**
java.awt.Color - De kleur om het gecensureerde gebied te vullen.

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


Stelt de kleur in om het geredigeerde gebied te vullen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.awt.Color | De kleur om het gecensureerde gebied te vullen. |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


Haalt de rechthoek met en hoogte op.


**Returns:**
java.awt.Dimension - De rechthoek met en hoogte.

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


Stelt de rechthoek met en hoogte in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.awt.Dimension | De rechthoek met en hoogte. |
|

