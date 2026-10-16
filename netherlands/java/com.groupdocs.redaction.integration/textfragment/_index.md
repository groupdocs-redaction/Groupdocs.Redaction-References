---
title: "TextFragment"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een deel van herkende tekst, woord, symbool enz. voor, geëxtraheerd door de OCR-engine."
type: docs
weight: 15
url: /nl/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

Stelt een deel van herkende tekst (woord, symbool, enz.) voor, geëxtraheerd door de OCR-engine.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | Initialiseert een nieuw exemplaar van het herkende tekstfragment. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getText()](#getText--) | Haalt de tekstuele inhoud van het herkende tekstfragment op. |
|
|  | [getRectangle()](#getRectangle--) | Haalt een begrenzende rechthoek van het herkende tekstfragment op. |
|
|  | [toString()](#toString--) | Retourneert de tekstuele inhoud van het herkende tekstfragment. |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


Initialiseert een nieuw exemplaar van het herkende tekstfragment.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | tekst | java.lang.String | tekstuele inhoud van het herkende tekstfragment |
|
|  | rectangle | java.awt.Rectangle | begrenzende rechthoek van het herkende tekstfragment |
|

### getText() {#getText--}
```
public final String getText()
```


Haalt de tekstuele inhoud van het herkende tekstfragment op.


**Returns:**
java.lang.String - Een tekstuele inhoud van het herkende tekstfragment.

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Haalt een begrenzende rechthoek van het herkende tekstfragment op.


**Returns:**
java.awt.Rectangle - Een begrenzende rechthoek van het herkende tekstfragment.

### toString() {#toString--}
```
public String toString()
```


Retourneert de tekstuele inhoud van het herkende tekstfragment.


**Returns:**
java.lang.String - tekstuele inhoud van het herkende tekstfragment

