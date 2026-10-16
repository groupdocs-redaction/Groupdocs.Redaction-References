---
title: "PageAreaFilter"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar ett raderingsfilter som anger ett område inom en sida i ett dokument för att tillämpa radering."
type: docs
weight: 22
url: /sv/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

Representerar ett redigeringsfilter som anger ett område inom en sida i ett dokument för att tillämpa redigering.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | Initierar en ny instans av PageAreaFilter-klassen för att radera ett specifikt område. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Hämtar rektangeln (övre vänstra positionen och storleken på området) på en sida. |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | Kontrollerar om detta filterområde har en skärning med den angivna rektangeln. |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


Initierar en ny instans av PageAreaFilter-klassen för att radera ett specifikt område.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Koordinater för övre vänstra området |
|
|  | storlek | java.awt.Dimension | Områdets storlek och färg |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Hämtar rektangeln (övre vänstra positionen och storleken på området) på en sida.


**Returns:**
java.awt.Rectangle - Rektangeln (övre vänstra positionen och storleken på området) på en sida.

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


Kontrollerar om detta filterområde har en skärning med den angivna rektangeln.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rektangel | java.awt.Rectangle | Rektangel att kontrollera |
|

**Returns:**
boolean - true, om detta filterområde har en skärning

