---
title: "TextLine"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en textrad som extraherats av OCR-motorn från en bild."
type: docs
weight: 16
url: /sv/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

Representerar en textrad, extraherad av OCR‑motorn från en bild.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | Initierar en ny instans av en textrad, extraherad av OCR-motorn från en bild. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFragments()](#getFragments--) | Hämtar en array av textfragment, såsom symboler och ord, som identifierats i raden. |
|
|  | [toString()](#toString--) | Returnerar textinnehåll för den igenkända textraden. |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


Initierar en ny instans av en textrad, extraherad av OCR-motorn från en bild.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | initial uppsättning av textfragment |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


Hämtar en array av textfragment, såsom symboler och ord, som identifierats i raden.


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - En array av textfragment, såsom symboler och ord, som identifierats i raden.

### toString() {#toString--}
```
public String toString()
```


Returnerar textinnehåll för den igenkända textraden.


**Returns:**
java.lang.String - textinnehåll för den igenkända textraden

