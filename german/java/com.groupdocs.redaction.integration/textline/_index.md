---
title: "TextLine"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt eine Textzeile dar, die von der OCR-Engine aus einem Bild extrahiert wurde."
type: docs
weight: 16
url: /de/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

Stellt eine Textzeile dar, die von der OCR-Engine aus einem Bild extrahiert wurde.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | Initialisiert eine neue Instanz einer Textzeile, die von der OCR-Engine aus einem Bild extrahiert wurde. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFragments()](#getFragments--) | Liefert ein Array von Textfragmenten, wie Symbolen und Wörtern, die in der Zeile erkannt wurden. |
|
|  | [toString()](#toString--) | Gibt den Textinhalt der erkannten Textzeile zurück. |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


Initialisiert eine neue Instanz einer Textzeile, die von der OCR-Engine aus einem Bild extrahiert wurde.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | initialer Satz von Textfragmenten |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


Liefert ein Array von Textfragmenten, wie Symbolen und Wörtern, die in der Zeile erkannt wurden.


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - Ein Array von Textfragmenten, wie Symbolen und Wörtern, die in der Zeile erkannt wurden.

### toString() {#toString--}
```
public String toString()
```


Gibt den Textinhalt der erkannten Textzeile zurück.


**Returns:**
java.lang.String - Textinhalt der erkannten Textzeile

