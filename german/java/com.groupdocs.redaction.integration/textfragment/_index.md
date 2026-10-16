---
title: "TextFragment"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt einen Teil des erkannten Textes, Wortes, Symbols usw. dar, das von der OCR-Engine extrahiert wurde."
type: docs
weight: 15
url: /de/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

Stellt einen Teil des erkannten Textes (Wort, Symbol usw.) dar, der von der OCR-Engine extrahiert wurde.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | Initialisiert eine neue Instanz des erkannten Textfragments. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getText()](#getText--) | Liefert den Textinhalt des erkannten Textfragments. |
|
|  | [getRectangle()](#getRectangle--) | Liefert das Begrenzungsrechteck des erkannten Textfragments. |
|
|  | [toString()](#toString--) | Gibt den Textinhalt des erkannten Textfragments zurück. |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


Initialisiert eine neue Instanz des erkannten Textfragments.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Text | java.lang.String | Textinhalt des erkannten Textfragments |
|
|  | rectangle | java.awt.Rectangle | Begrenzungsrechteck des erkannten Textfragments |
|

### getText() {#getText--}
```
public final String getText()
```


Liefert den Textinhalt des erkannten Textfragments.


**Returns:**
java.lang.String - Ein Textinhalt des erkannten Textfragments.

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Liefert das Begrenzungsrechteck des erkannten Textfragments.


**Returns:**
java.awt.Rectangle - Ein Begrenzungsrechteck des erkannten Textfragments.

### toString() {#toString--}
```
public String toString()
```


Gibt den Textinhalt des erkannten Textfragments zurück.


**Returns:**
java.lang.String - Textinhalt des erkannten Textfragments

