---
title: "RecognizedImage"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt tekst voor die uit een afbeelding is gehaald als resultaat van het herkenningsproces."
type: docs
weight: 13
url: /nl/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

Stelt tekst voor, geëxtraheerd uit een afbeelding als resultaat van het herkenningsproces.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | Initialiseert een nieuw exemplaar van de klasse, met behulp van een set van herkende regels. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getText()](#getText--) | Haalt de tekstuele equivalent op van de gestructureerde tekst. |
|
|  | [getLines()](#getLines--) | Haalt regels tekst op, met hun fragmenten, die binnen het document zijn herkend. |
|
|  | [toString()](#toString--) | Haalt de tekstuele equivalent op van de gestructureerde tekst. |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


Initialiseert een nieuw exemplaar van de klasse, met behulp van een set van herkende regels.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | een IEnumerable (bijv. een lijst of een array) van herkende regels |
|

### getText() {#getText--}
```
public final String getText()
```


Haalt de tekstuele equivalent op van de gestructureerde tekst.


**Returns:**
java.lang.String - Tekstuele equivalent van de gestructureerde tekst.

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


Haalt regels tekst op, met hun fragmenten, die binnen het document zijn herkend.


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - Regels tekst, met hun fragmenten, die binnen het document zijn herkend.

### toString() {#toString--}
```
public String toString()
```


Haalt de tekstuele equivalent op van de gestructureerde tekst.


**Returns:**
java.lang.String - Herkende tekst

