---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een redactiestrategie voor die een gekleurde rechthoek plaatst in een opgegeven gebied van een beelddocument."
type: docs
weight: 18
url: /nl/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

Stelt een redactiestrategie voor die een gekleurde rechthoek plaatst in een opgegeven gebied van een beelddocument.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Initialiseert een nieuw exemplaar van de ImageAreaRedaction-klasse om een specifiek gebied te redigeren. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getOptions()](#getOptions--) | Haalt de |
RegionReplacementOptions
opties met kleur- en gebiedsparameters.
|
|  | [getTopLeft()](#getTopLeft--) | Haalt de linkerbovenhoekpositie van het te verwijderen gebied op |
|
|  | [getDescription()](#getDescription--) | Retourneert een string die de redactie en de parameters beschrijft. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Past de redactie toe op een gegeven formaatinstantie. |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


Initialiseert een nieuw exemplaar van de ImageAreaRedaction-klasse om een specifiek gebied te redigeren.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Coördinaten van het linkerbovengebied |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Grootte en kleur van het gebied |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


Haalt de
RegionReplacementOptions
opties met kleur- en gebiedsparameters.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


Haalt de linkerbovenhoekpositie van het te verwijderen gebied op


**Returns:**
java.awt.Point - De linkerbovenhoekpositie van het te verwijderen gebied

### getDescription() {#getDescription--}
```
public String getDescription()
```


Retourneert een string die de redactie en de parameters beschrijft.


**Returns:**
java.lang.String - Tekst die de naam van de redactie en parameters bevat.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Past de redactie toe op een gegeven formaatinstantie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Een instantie van een document om redactie toe te passen |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

