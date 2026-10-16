---
title: "ExactPhraseRedaction"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente un masquage de texte qui remplace une phrase exacte dans le texte du document, insensible à la casse par défaut."
type: docs
weight: 17
url: /fr/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

Représente une rédaction de texte qui remplace une phrase exacte dans le texte du document, insensible à la casse par défaut.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

L'exemple suivant montre comment effectuer une recherche et un remplacement de phrase sensibles à la casse.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
``` 
````

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

````

try (Redactor redactor = new Redactor("C:\\sample.pdf"))
{
// Par défaut, isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));

doc.save();
}
 
``` 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialise une nouvelle instance de la classe ExactPhraseRedaction en mode insensible à la casse. |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialise une nouvelle instance de la classe ExactPhraseRedaction. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | Obtient la chaîne à rechercher et remplacer. |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | Obtient une valeur indiquant si la recherche est sensible à la casse ou non. |
|
|  | [isRightToLeft()](#isRightToLeft--) | Obtient une valeur indiquant si ce texte est de droite à gauche ou non, false par défaut. |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | Définit une valeur indiquant si ce texte est de droite à gauche ou non, false par défaut. |
|
|  | [getDescription()](#getDescription--) | Renvoie une chaîne, décrivant la rédaction et ses paramètres. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applique la rédaction à une instance de format donnée. |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


Initialise une nouvelle instance de la classe ExactPhraseRedaction en mode insensible à la casse.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Chaîne à rechercher et remplacer |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Options de remplacement (textuel, couleur) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


Initialise une nouvelle instance de la classe ExactPhraseRedaction.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Chaîne à rechercher et remplacer |
|
|  | isCaseSensitive | boolean | True si une recherche sensible à la casse est requise |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Options de remplacement (textuel, couleur) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


Obtient la chaîne à rechercher et remplacer.


**Returns:**
java.lang.String - La chaîne à rechercher et remplacer.

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


Obtient une valeur indiquant si la recherche est sensible à la casse ou non.


**Returns:**
boolean - Une valeur indiquant si la recherche est sensible à la casse ou non.

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


Obtient une valeur indiquant si ce texte est de droite à gauche ou non, false par défaut.


**Returns:**
boolean - Une valeur indiquant si ce texte est de droite à gauche ou non, false par défaut.

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


Définit une valeur indiquant si ce texte est de droite à gauche ou non, false par défaut.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant si ce texte est de droite à gauche ou non, false par défaut. |
|

### getDescription() {#getDescription--}
```
public String getDescription()
```


Renvoie une chaîne, décrivant la rédaction et ses paramètres.


**Returns:**
java.lang.String - Texte contenant le nom de la rédaction et les paramètres.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applique la rédaction à une instance de format donnée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Une instance d'un document pour appliquer la rédaction |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

