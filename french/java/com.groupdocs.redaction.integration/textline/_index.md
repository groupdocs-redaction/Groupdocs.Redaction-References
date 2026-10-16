---
title: "TextLine"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente une ligne de texte extraite par le moteur OCR à partir d'une image."
type: docs
weight: 16
url: /fr/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

Représente une ligne de texte, extraite par le moteur OCR d'une image.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | Initialise une nouvelle instance d'une ligne de texte, extraite par le moteur OCR à partir d'une image. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getFragments()](#getFragments--) | Obtient un tableau de fragments de texte, tels que des symboles et des mots, reconnus dans la ligne. |
|
|  | [toString()](#toString--) | Renvoie le contenu textuel de la ligne de texte reconnue. |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


Initialise une nouvelle instance d'une ligne de texte, extraite par le moteur OCR à partir d'une image.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | ensemble initial de fragments de texte |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


Obtient un tableau de fragments de texte, tels que des symboles et des mots, reconnus dans la ligne.


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - Un tableau de fragments de texte, tels que des symboles et des mots, reconnus dans la ligne.

### toString() {#toString--}
```
public String toString()
```


Renvoie le contenu textuel de la ligne de texte reconnue.


**Returns:**
java.lang.String - contenu textuel de la ligne de texte reconnue

