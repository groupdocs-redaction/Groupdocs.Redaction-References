---
title: "Redaction"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta una classe astratta di base per tutti i tipi di redazione."
type: docs
weight: 13
url: /it/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

Rappresenta una classe astratta di base per tutti i tipi di redazione.

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getDescription()](#getDescription--) | Restituisce una stringa che descrive la redazione e i suoi parametri. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applica la redazione a una determinata istanza di formato. |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


Restituisce una stringa che descrive la redazione e i suoi parametri.


**Returns:**
java.lang.String - Testo, contenente il nome della redazione e i parametri.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applica la redazione a una determinata istanza di formato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Un'istanza di un documento a cui applicare la redazione |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

