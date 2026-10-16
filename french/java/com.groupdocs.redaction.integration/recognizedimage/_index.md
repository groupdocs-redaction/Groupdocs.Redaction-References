---
title: "RecognizedImage"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente le texte extrait d'une image à la suite de son processus de reconnaissance."
type: docs
weight: 13
url: /fr/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

Représente du texte, extrait d'une image à la suite de son processus de reconnaissance.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | Initialise une nouvelle instance de la classe, en utilisant un ensemble de lignes reconnues. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getText()](#getText--) | Obtient l'équivalent textuel du texte structuré. |
|
|  | [getLines()](#getLines--) | Obtient les lignes de texte, avec leurs fragments, reconnues dans le document. |
|
|  | [toString()](#toString--) | Obtient l'équivalent textuel du texte structuré. |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


Initialise une nouvelle instance de la classe, en utilisant un ensemble de lignes reconnues.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | un IEnumerable (par ex. une liste ou un tableau) de lignes reconnues |
|

### getText() {#getText--}
```
public final String getText()
```


Obtient l'équivalent textuel du texte structuré.


**Returns:**
java.lang.String - Équivalent textuel du texte structuré.

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


Obtient les lignes de texte, avec leurs fragments, reconnues dans le document.


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - Lignes de texte, avec leurs fragments, reconnues dans le document.

### toString() {#toString--}
```
public String toString()
```


Obtient l'équivalent textuel du texte structuré.


**Returns:**
java.lang.String - Texte reconnu

