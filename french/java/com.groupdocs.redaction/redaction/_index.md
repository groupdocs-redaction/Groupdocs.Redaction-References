---
title: "Rédaction"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente une classe abstraite de base pour tous les types de rédaction."
type: docs
weight: 13
url: /fr/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

Représente une classe abstraite de base pour tous les types de rédaction.

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getDescription()](#getDescription--) | Renvoie une chaîne, décrivant la rédaction et ses paramètres. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applique la rédaction à une instance de format donnée. |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


Renvoie une chaîne, décrivant la rédaction et ses paramètres.


**Returns:**
java.lang.String - Texte contenant le nom de la rédaction et les paramètres.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applique la rédaction à une instance de format donnée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Une instance d'un document pour appliquer la rédaction |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

