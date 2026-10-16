---
title: "PageAreaFilter"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een redactiefilter voor dat een gebied binnen een pagina van een document instelt om redactie toe te passen."
type: docs
weight: 22
url: /nl/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

Vertegenwoordigt een redactiefilter dat een gebied binnen een pagina van een document instelt om redacties toe te passen.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | Initialiseert een nieuw exemplaar van de PageAreaFilter‑klasse voor het redigeren van een specifiek gebied. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Haalt de rechthoek (linkerbovenpositie en grootte van het gebied) op een pagina op. |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | Controleert of dit filtergebied intersectie heeft met de opgegeven rechthoek. |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


Initialiseert een nieuw exemplaar van de PageAreaFilter‑klasse voor het redigeren van een specifiek gebied.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Coördinaten van het linkerbovengebied |
|
|  | size | java.awt.Dimension | Grootte en kleur van het gebied |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Haalt de rechthoek (linkerbovenpositie en grootte van het gebied) op een pagina op.


**Returns:**
java.awt.Rectangle - De rechthoek (linkerbovenpositie en grootte van het gebied) op een pagina.

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


Controleert of dit filtergebied intersectie heeft met de opgegeven rechthoek.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | java.awt.Rectangle | Rechthoek om te controleren |
|

**Returns:**
boolean - true, als dit filtergebied intersectie heeft

