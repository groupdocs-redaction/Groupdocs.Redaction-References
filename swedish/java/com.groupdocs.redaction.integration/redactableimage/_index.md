---
title: "RedactableImage"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Tillhandahåller en fasad till alla rasterbildsredigeringsoperationer."
type: docs
weight: 14
url: /sv/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

Tillhandahåller en fasad till alla rasterbildsredigeringsoperationer.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | Skapar en ny instans med ett objekt som implementerar |
IImageFormatInstance
gränssnitt.
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | Skapar en ny instans med ett objekt som implementerar |
IMultipleAreaRedactable
gränssnitt.
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | Hämtar en ström med faktiskt bildinnehåll. |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Raderar flera bildområden på en gång med samma färg. |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Ersätter området vid given punkt med en rektangel av specifik färg och storlek. |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


Skapar en ny instans med ett objekt som implementerar
IImageFormatInstance
gränssnitt.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | En instans som implementerar IImageFormatInstance‑gränssnittet |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


Skapar en ny instans med ett objekt som implementerar
IMultipleAreaRedactable
gränssnitt.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | En instans som implementerar IMultipleAreaRedactable‑gränssnittet |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


Hämtar en ström med faktiskt bildinnehåll.


**Returns:**
java.io.InputStream - Ström som innehåller bilddata

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


Raderar flera bildområden på en gång med samma färg.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rektanglar | java.awt.Rectangle[] | En array av rektangelområden |
|
|  | boxColor | java.awt.Color | Färg för att fylla områdena |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Ersätter området vid given punkt med en rektangel av specifik färg och storlek.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Koordinater för övre vänstra hörnet på det fyllda området |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Färg- och storleksinställningar |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

