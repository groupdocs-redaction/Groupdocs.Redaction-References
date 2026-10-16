---
title: "TextFragment"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en del av igenkänd text, ord, symbol etc. som extraherats av OCR-motorn."
type: docs
weight: 15
url: /sv/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

Representerar en del av igenkänd text (ord, symbol osv), extraherad av OCR‑motorn.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | Initierar en ny instans av den igenkända textfragmentet. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getText()](#getText--) | Hämtar ett textinnehåll för det igenkända textfragmentet. |
|
|  | [getRectangle()](#getRectangle--) | Hämtar en avgränsande rektangel för det igenkända textfragmentet. |
|
|  | [toString()](#toString--) | Returnerar textinnehåll för det igenkända textfragmentet. |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


Initierar en ny instans av den igenkända textfragmentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | text | java.lang.String | textinnehåll för det igenkända textfragmentet |
|
|  | rektangel | java.awt.Rectangle | avgränsande rektangel för det igenkända textfragmentet |
|

### getText() {#getText--}
```
public final String getText()
```


Hämtar ett textinnehåll för det igenkända textfragmentet.


**Returns:**
java.lang.String - Ett textinnehåll för det igenkända textfragmentet.

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Hämtar en avgränsande rektangel för det igenkända textfragmentet.


**Returns:**
java.awt.Rectangle - En avgränsande rektangel för det igenkända textfragmentet.

### toString() {#toString--}
```
public String toString()
```


Returnerar textinnehåll för det igenkända textfragmentet.


**Returns:**
java.lang.String - textinnehåll för det igenkända textfragmentet

