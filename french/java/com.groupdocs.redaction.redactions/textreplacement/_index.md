---
title: "TextReplacement"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente une information de remplacement textuel."
type: docs
weight: 33
url: /fr/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

Représente une information de remplacement textuel.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | Initialise une nouvelle instance de la classe TextReplacement. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getIndex()](#getIndex--) | Obtient l'index du texte correspondant dans la chaîne source. |
|
|  | [getOriginalText()](#getOriginalText--) | Obtient la chaîne originale correspondante. |
|
|  | [getReplacement()](#getReplacement--) | Obtient la chaîne, en remplaçant OriginalText. |
|
|  | [toString()](#toString--) | Fournit la description du remplacement de texte et sa position. |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


Initialise une nouvelle instance de la classe TextReplacement.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | index | int | Index d'un texte correspondant dans la chaîne source |
|
|  | original | java.lang.String | Chaîne correspondante originale |
|
|  | remplacement | java.lang.String | Chaîne, remplaçant OriginalText dans la chaîne source |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Obtient l'index du texte correspondant dans la chaîne source.


**Returns:**
int - Un index du texte correspondant dans la chaîne source.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Obtient la chaîne originale correspondante.


**Returns:**
java.lang.String - La chaîne correspondante originale.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Obtient la chaîne, en remplaçant OriginalText.


**Returns:**
java.lang.String - La chaîne, remplaçant OriginalText.

### toString() {#toString--}
```
public String toString()
```


Fournit la description du remplacement de texte et sa position.


**Returns:**
java.lang.String - Description du remplacement

