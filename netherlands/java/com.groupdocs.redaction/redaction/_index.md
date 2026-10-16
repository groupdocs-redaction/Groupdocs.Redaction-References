---
title: "Redaction"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een basis abstracte klasse voor alle redactietypen voor."
type: docs
weight: 13
url: /nl/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

Stelt een basis abstracte klasse voor alle redactietypen voor.

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getDescription()](#getDescription--) | Retourneert een string die de redactie en de parameters beschrijft. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Past de redactie toe op een gegeven formaatinstantie. |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


Retourneert een string die de redactie en de parameters beschrijft.


**Returns:**
java.lang.String - Tekst die de naam van de redactie en parameters bevat.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Past de redactie toe op een gegeven formaatinstantie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Een instantie van een document om redactie toe te passen |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

