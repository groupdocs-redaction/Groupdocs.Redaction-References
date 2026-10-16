---
title: "TextLine"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een regel tekst voor die door de OCR-engine uit een afbeelding is gehaald."
type: docs
weight: 16
url: /nl/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

Stelt een regel tekst voor, geëxtraheerd door de OCR-engine uit een afbeelding.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | Initialiseert een nieuw exemplaar van een regel tekst, geëxtraheerd door de OCR-engine uit een afbeelding. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFragments()](#getFragments--) | Haalt een array van tekstfragmenten op, zoals symbolen en woorden, die in de regel zijn herkend. |
|
|  | [toString()](#toString--) | Retourneert de tekstuele inhoud van de herkende tekstregel. |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


Initialiseert een nieuw exemplaar van een regel tekst, geëxtraheerd door de OCR-engine uit een afbeelding.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | initiële set van tekstfragmenten |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


Haalt een array van tekstfragmenten op, zoals symbolen en woorden, die in de regel zijn herkend.


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - Een array van tekstfragmenten, zoals symbolen en woorden, die in de regel zijn herkend.

### toString() {#toString--}
```
public String toString()
```


Retourneert de tekstuele inhoud van de herkende tekstregel.


**Returns:**
java.lang.String - tekstuele inhoud van de herkende tekstregel

