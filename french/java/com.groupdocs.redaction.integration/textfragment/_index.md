---
title: "TextFragment"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente une partie du texte reconnu, mot, symbole, etc., extrait par le moteur OCR."
type: docs
weight: 15
url: /fr/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

Représente une partie du texte reconnu (mot, symbole, etc.), extrait par le moteur OCR.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | Initialise une nouvelle instance du fragment de texte reconnu. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getText()](#getText--) | Obtient le contenu textuel du fragment de texte reconnu. |
|
|  | [getRectangle()](#getRectangle--) | Obtient le rectangle englobant du fragment de texte reconnu. |
|
|  | [toString()](#toString--) | Renvoie le contenu textuel du fragment de texte reconnu. |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


Initialise une nouvelle instance du fragment de texte reconnu.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | texte | java.lang.String | contenu textuel du fragment de texte reconnu |
|
|  | rectangle | java.awt.Rectangle | rectangle englobant du fragment de texte reconnu |
|

### getText() {#getText--}
```
public final String getText()
```


Obtient le contenu textuel du fragment de texte reconnu.


**Returns:**
java.lang.String - Un contenu textuel du fragment de texte reconnu.

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Obtient le rectangle englobant du fragment de texte reconnu.


**Returns:**
java.awt.Rectangle - Un rectangle englobant du fragment de texte reconnu.

### toString() {#toString--}
```
public String toString()
```


Renvoie le contenu textuel du fragment de texte reconnu.


**Returns:**
java.lang.String - contenu textuel du fragment de texte reconnu

