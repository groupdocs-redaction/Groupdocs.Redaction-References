---
title: "TextReplacement"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Informationen zum textuellen Austausch dar."
type: docs
weight: 33
url: /de/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

Stellt Informationen zum textuellen Austausch dar.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | Initialisiert eine neue Instanz der Klasse TextReplacement. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getIndex()](#getIndex--) | Gibt den Index des gefundenen Textes im Quellstring zurück. |
|
|  | [getOriginalText()](#getOriginalText--) | Gibt die ursprünglich gefundene Zeichenkette zurück. |
|
|  | [getReplacement()](#getReplacement--) | Gibt die Zeichenkette zurück, die OriginalText ersetzt. |
|
|  | [toString()](#toString--) | Stellt die Beschreibung des Textaustauschs und dessen Position bereit. |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


Initialisiert eine neue Instanz der Klasse TextReplacement.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Index | int | Index eines gefundenen Textes im Quellstring |
|
|  | original | java.lang.String | Ursprünglich gefundene Zeichenkette |
|
|  | Ersetzung | java.lang.String | Zeichenkette, die OriginalText im Quellstring ersetzt |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Gibt den Index des gefundenen Textes im Quellstring zurück.


**Returns:**
int - Ein Index des gefundenen Textes im Quellstring.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Gibt die ursprünglich gefundene Zeichenkette zurück.


**Returns:**
java.lang.String - Die ursprünglich gefundene Zeichenkette.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Gibt die Zeichenkette zurück, die OriginalText ersetzt.


**Returns:**
java.lang.String - Die Zeichenkette, die OriginalText ersetzt.

### toString() {#toString--}
```
public String toString()
```


Stellt die Beschreibung des Textaustauschs und dessen Position bereit.


**Returns:**
java.lang.String - Beschreibung des Austauschs

