---
title: "TextReplacement"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta le informazioni di una sostituzione testuale."
type: docs
weight: 33
url: /it/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

Rappresenta le informazioni di una sostituzione testuale.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | Inizializza una nuova istanza della classe TextReplacement. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getIndex()](#getIndex--) | Ottiene un indice del testo corrispondente all'interno della stringa di origine. |
|
|  | [getOriginalText()](#getOriginalText--) | Ottiene la stringa originale corrispondente. |
|
|  | [getReplacement()](#getReplacement--) | Ottiene la stringa, sostituendo OriginalText. |
|
|  | [toString()](#toString--) | Fornisce la descrizione della sostituzione del testo e la sua posizione. |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


Inizializza una nuova istanza della classe TextReplacement.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indice | int | Indice di un testo corrispondente all'interno della stringa di origine |
|
|  | originale | java.lang.String | Stringa originale corrispondente |
|
|  | sostituzione | java.lang.String | Stringa, sostituendo OriginalText nella stringa di origine |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Ottiene un indice del testo corrispondente all'interno della stringa di origine.


**Returns:**
int - Un indice del testo corrispondente all'interno della stringa di origine.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Ottiene la stringa originale corrispondente.


**Returns:**
java.lang.String - La stringa originale corrispondente.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Ottiene la stringa, sostituendo OriginalText.


**Returns:**
java.lang.String - La stringa, sostituendo OriginalText.

### toString() {#toString--}
```
public String toString()
```


Fornisce la descrizione della sostituzione del testo e la sua posizione.


**Returns:**
java.lang.String - Descrizione della sostituzione

