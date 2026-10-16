---
title: "TextReplacement"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Vertegenwoordigt informatie over een tekstuele vervanging."
type: docs
weight: 33
url: /nl/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

Vertegenwoordigt informatie over een tekstuele vervanging.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | Initialiseert een nieuw exemplaar van de TextReplacement-klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getIndex()](#getIndex--) | Haalt een index op van de overeenkomende tekst binnen de brontekenreeks. |
|
|  | [getOriginalText()](#getOriginalText--) | Haalt de oorspronkelijke overeenkomende tekenreeks op. |
|
|  | [getReplacement()](#getReplacement--) | Haalt de string op, vervangt OriginalText. |
|
|  | [toString()](#toString--) | Biedt een beschrijving van de tekstvervanging en de positie ervan. |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


Initialiseert een nieuw exemplaar van de TextReplacement-klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | index | int | Index van een overeenkomende tekst binnen de bronstring |
|
|  | origineel | java.lang.String | Originele overeenkomende string |
|
|  | vervanging | java.lang.String | String, vervangt OriginalText in de bronstring |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Haalt een index op van de overeenkomende tekst binnen de brontekenreeks.


**Returns:**
int - Een index van de overeenkomende tekst binnen de bronstring.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Haalt de oorspronkelijke overeenkomende tekenreeks op.


**Returns:**
java.lang.String - De originele overeenkomende string.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Haalt de string op, vervangt OriginalText.


**Returns:**
java.lang.String - De string, vervangt OriginalText.

### toString() {#toString--}
```
public String toString()
```


Biedt een beschrijving van de tekstvervanging en de positie ervan.


**Returns:**
java.lang.String - Beschrijving van vervanging

