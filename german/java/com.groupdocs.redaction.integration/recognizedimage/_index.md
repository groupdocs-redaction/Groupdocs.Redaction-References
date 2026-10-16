---
title: "RecognizedImage"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Text dar, der aus einem Bild als Ergebnis seines Erkennungsprozesses extrahiert wurde."
type: docs
weight: 13
url: /de/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

Stellt Text dar, der aus einem Bild als Ergebnis seines Erkennungsprozesses extrahiert wurde.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | Initialisiert eine neue Instanz der Klasse unter Verwendung einer Menge erkannter Zeilen. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getText()](#getText--) | Gibt das textuelle Äquivalent des strukturierten Textes zurück. |
|
|  | [getLines()](#getLines--) | Gibt Textzeilen mit ihren Fragmenten zurück, die im Dokument erkannt wurden. |
|
|  | [toString()](#toString--) | Gibt das textuelle Äquivalent des strukturierten Textes zurück. |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


Initialisiert eine neue Instanz der Klasse unter Verwendung einer Menge erkannter Zeilen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | ein IEnumerable (z. B. eine Liste oder ein Array) von erkannten Zeilen |
|

### getText() {#getText--}
```
public final String getText()
```


Gibt das textuelle Äquivalent des strukturierten Textes zurück.


**Returns:**
java.lang.String - Textuelles Äquivalent des strukturierten Textes.

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


Gibt Textzeilen mit ihren Fragmenten zurück, die im Dokument erkannt wurden.


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - Textzeilen mit ihren Fragmenten, die im Dokument erkannt wurden.

### toString() {#toString--}
```
public String toString()
```


Gibt das textuelle Äquivalent des strukturierten Textes zurück.


**Returns:**
java.lang.String - Erkennter Text

