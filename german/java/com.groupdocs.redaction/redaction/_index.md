---
title: "Redaction"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt eine Basis-abstrakte Klasse für alle Redaktionsarten dar."
type: docs
weight: 13
url: /de/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

Stellt eine Basis-abstrakte Klasse für alle Redaktionsarten dar.

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getDescription()](#getDescription--) | Gibt eine Zeichenkette zurück, die die Redaktion und ihre Parameter beschreibt. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


Gibt eine Zeichenkette zurück, die die Redaktion und ihre Parameter beschreibt.


**Returns:**
java.lang.String - Text, der den Namen der Redaktion und Parameter enthält.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Wendet die Redaktion auf eine gegebene Formatinstanz an.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Eine Instanz eines Dokuments, auf das die Redaktion angewendet wird |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

