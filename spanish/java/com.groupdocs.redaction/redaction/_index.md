---
title: "Redaction"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una clase abstracta base para todos los tipos de redacción."
type: docs
weight: 13
url: /es/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

Representa una clase abstracta base para todos los tipos de redacción.

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getDescription()](#getDescription--) | Devuelve una cadena que describe la redacción y sus parámetros. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Aplica la redacción a una instancia de formato dada. |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


Devuelve una cadena que describe la redacción y sus parámetros.


**Returns:**
java.lang.String - Texto que contiene el nombre de la redacción y los parámetros.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Aplica la redacción a una instancia de formato dada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Una instancia de un documento para aplicar la redacción |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

