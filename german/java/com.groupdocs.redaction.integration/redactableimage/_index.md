---
title: "RedactableImage"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Bietet eine Fassade für alle Rasterbild-Redaktionsvorgänge."
type: docs
weight: 14
url: /de/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

Bietet eine Fassade für alle Rasterbild-Redaktionsvorgänge.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | Erstellt eine neue Instanz unter Verwendung eines Objekts, das implementiert |
IImageFormatInstance
Schnittstelle.
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | Erstellt eine neue Instanz unter Verwendung eines Objekts, das implementiert |
IMultipleAreaRedactable
Schnittstelle.
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | Ruft einen Stream mit dem tatsächlichen Bildinhalt ab. |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Redigiert mehrere Bildbereiche gleichzeitig mit derselben Farbe. |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Ersetzt den Bereich an einem gegebenen Punkt durch ein Rechteck mit spezifischer Farbe und Größe. |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


Erstellt eine neue Instanz unter Verwendung eines Objekts, das implementiert
IImageFormatInstance
Schnittstelle.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | Eine Instanz, die das IImageFormatInstance-Interface implementiert |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


Erstellt eine neue Instanz unter Verwendung eines Objekts, das implementiert
IMultipleAreaRedactable
Schnittstelle.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | Eine Instanz, die das Interface IMultipleAreaRedactable implementiert |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


Ruft einen Stream mit dem tatsächlichen Bildinhalt ab.


**Returns:**
java.io.InputStream - Stream, der Bilddaten enthält

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


Redigiert mehrere Bildbereiche gleichzeitig mit derselben Farbe.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Rechtecke | java.awt.Rectangle[] | Ein Array von Rechteckbereichen |
|
|  | boxColor | java.awt.Color | Farbe zum Füllen der Bereiche |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Ersetzt den Bereich an einem gegebenen Punkt durch ein Rechteck mit spezifischer Farbe und Größe.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Koordinaten der oberen linken Ecke des gefüllten Bereichs |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Farbe- und Größeneinstellungen |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

