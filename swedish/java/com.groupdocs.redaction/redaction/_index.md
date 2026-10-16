---
title: "Redigering"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en grundläggande abstrakt klass för alla raderingsklasser."
type: docs
weight: 13
url: /sv/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

Representerar en grundläggande abstrakt klass för alla raderingsklasser.

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getDescription()](#getDescription--) | Returnerar en sträng som beskriver redigeringen och dess parametrar. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Tillämpar redigeringen på en given formatinstans. |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


Returnerar en sträng som beskriver redigeringen och dess parametrar.


**Returns:**
java.lang.String - Text som innehåller redigeringsnamn och parametrar.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Tillämpar redigeringen på en given formatinstans.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | En instans av ett dokument för att tillämpa redigering |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

