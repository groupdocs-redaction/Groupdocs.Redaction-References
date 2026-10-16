---
title: "RegexRedaction"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente une rédaction de texte qui recherche et remplace le texte dans le document en faisant correspondre l'expression régulière fournie."
type: docs
weight: 28
url: /fr/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

Représente une rédaction de texte qui recherche et remplace le texte dans le document en faisant correspondre l'expression régulière fournie.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialise une nouvelle instance de la classe RegexRedaction. |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialise une nouvelle instance de la classe RegexRedaction. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | Obtient l'expression régulière à faire correspondre. |
|
|  | [getDescription()](#getDescription--) | Renvoie une chaîne, décrivant la rédaction et ses paramètres. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applique la rédaction à une instance de format donnée. |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


Initialise une nouvelle instance de la classe RegexRedaction.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | modèle | java.lang.String | Expression régulière pour rechercher et remplacer |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Options de remplacement (textuel, couleur) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


Initialise une nouvelle instance de la classe RegexRedaction.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Expression régulière pour rechercher et remplacer |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Options de remplacement (textuel, couleur) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


Obtient l'expression régulière à faire correspondre.


**Returns:**
java.util.regex.Pattern - L'expression régulière à faire correspondre.

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

