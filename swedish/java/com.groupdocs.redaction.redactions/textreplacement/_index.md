---
title: "TextReplacement"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar information om en textuell ersättning."
type: docs
weight: 33
url: /sv/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

Representerar information om en textuell ersättning.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | Initierar en ny instans av klassen TextReplacement. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getIndex()](#getIndex--) | Hämtar ett index för den matchade texten i källsträngen. |
|
|  | [getOriginalText()](#getOriginalText--) | Hämtar den ursprungliga matchade strängen. |
|
|  | [getReplacement()](#getReplacement--) | Hämtar strängen som ersätter OriginalText. |
|
|  | [toString()](#toString--) | Tillhandahåller beskrivning av textersättning och dess position. |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


Initierar en ny instans av klassen TextReplacement.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | int | Index för en matchad text i källsträngen |
|
|  | original | java.lang.String | Original matchad sträng |
|
|  | ersättning | java.lang.String | Sträng som ersätter OriginalText i källsträngen |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Hämtar ett index för den matchade texten i källsträngen.


**Returns:**
int - Ett index för den matchade texten i källsträngen.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Hämtar den ursprungliga matchade strängen.


**Returns:**
java.lang.String - Den originala matchade strängen.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Hämtar strängen som ersätter OriginalText.


**Returns:**
java.lang.String - Strängen som ersätter OriginalText.

### toString() {#toString--}
```
public String toString()
```


Tillhandahåller beskrivning av textersättning och dess position.


**Returns:**
java.lang.String - Beskrivning av ersättning

