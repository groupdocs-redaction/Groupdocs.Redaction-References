---
title: "RecognizedImage"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar text som extraherats från en bild som ett resultat av dess igenkänningsprocess."
type: docs
weight: 13
url: /sv/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

Representerar text som extraheras från en bild som resultat av dess igenkänningsprocess.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | Initierar en ny instans av klassen med en uppsättning igenkända rader. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getText()](#getText--) | Hämtar den textuella motsvarigheten till den strukturerade texten. |
|
|  | [getLines()](#getLines--) | Hämtar rader av text, med deras fragment, som känns igen i dokumentet. |
|
|  | [toString()](#toString--) | Hämtar den textuella motsvarigheten till den strukturerade texten. |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


Initierar en ny instans av klassen med en uppsättning igenkända rader.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | en IEnumerable (t.ex. en lista eller en array) av igenkända rader |
|

### getText() {#getText--}
```
public final String getText()
```


Hämtar den textuella motsvarigheten till den strukturerade texten.


**Returns:**
java.lang.String - Textuell motsvarighet till den strukturerade texten.

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


Hämtar rader av text, med deras fragment, som känns igen i dokumentet.


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - Rader av text, med deras fragment, som känns igen i dokumentet.

### toString() {#toString--}
```
public String toString()
```


Hämtar den textuella motsvarigheten till den strukturerade texten.


**Returns:**
java.lang.String - Igenkänd text

