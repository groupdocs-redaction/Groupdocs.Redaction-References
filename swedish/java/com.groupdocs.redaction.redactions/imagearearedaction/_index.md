---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en radering som placerar en färgad rektangel i ett givet område av ett bilddokument."
type: docs
weight: 18
url: /sv/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

Representerar en radering som placerar en färgad rektangel i ett givet område av ett bilddokument.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Initierar en ny instans av ImageAreaRedaction-klassen för att radera ett specifikt område. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getOptions()](#getOptions--) | Hämtar |
RegionReplacementOptions
alternativ med färg- och områdesparametrar.
|
|  | [getTopLeft()](#getTopLeft--) | Hämtar den övre vänstra positionen för området som ska tas bort |
|
|  | [getDescription()](#getDescription--) | Returnerar en sträng som beskriver redigeringen och dess parametrar. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Tillämpar redigeringen på en given formatinstans. |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


Initierar en ny instans av ImageAreaRedaction-klassen för att radera ett specifikt område.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Koordinater för övre vänstra området |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Områdets storlek och färg |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


Hämtar
RegionReplacementOptions
alternativ med färg- och områdesparametrar.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


Hämtar den övre vänstra positionen för området som ska tas bort


**Returns:**
java.awt.Point - Den övre vänstra positionen för området som ska tas bort

### getDescription() {#getDescription--}
```
public String getDescription()
```


Returnerar en sträng som beskriver redigeringen och dess parametrar.


**Returns:**
java.lang.String - Text som innehåller redigeringsnamn och parametrar.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Tillämpar redigeringen på en given formatinstans.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | En instans av ett dokument för att tillämpa redigering |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

