---
title: "RedactableImage"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Biedt een façade voor alle rasterafbeelding-redactiebewerkingen."
type: docs
weight: 14
url: /nl/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

Biedt een façade voor alle rasterafbeelding-redactiebewerkingen.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | Maakt een nieuw exemplaar aan met een object, dat implementeert |
IImageFormatInstance
interface.
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | Maakt een nieuw exemplaar aan met een object, dat implementeert |
IMultipleAreaRedactable
interface.
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | Haalt een stream op met de daadwerkelijke afbeeldingsinhoud. |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Redigeert meerdere afbeeldingsgebieden tegelijk met dezelfde kleur. |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Vervangt het gebied op een gegeven punt door een rechthoek met een specifieke kleur en grootte. |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


Maakt een nieuw exemplaar aan met een object, dat implementeert
IImageFormatInstance
interface.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | Een exemplaar, dat de IImageFormatInstance-interface implementeert |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


Maakt een nieuw exemplaar aan met een object, dat implementeert
IMultipleAreaRedactable
interface.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | Een exemplaar, dat de IMultipleAreaRedactable-interface implementeert |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


Haalt een stream op met de daadwerkelijke afbeeldingsinhoud.


**Returns:**
java.io.InputStream - Stream, die afbeeldingsgegevens bevat

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


Redigeert meerdere afbeeldingsgebieden tegelijk met dezelfde kleur.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rechthoeken | java.awt.Rectangle[] | Een array van rechthoekgebieden |
|
|  | boxColor | java.awt.Color | Kleur om de gebieden te vullen |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Vervangt het gebied op een gegeven punt door een rechthoek met een specifieke kleur en grootte.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Coördinaten van de linkerbovenhoek van het gevulde gebied |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Kleur- en grootte-instellingen |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

