---
title: "RedactorLogEntry"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta i risultati dell'applicazione della redazione."
type: docs
weight: 18
url: /it/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

Rappresenta i risultati dell'applicazione della redazione.

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | Inizializza una nuova istanza della classe RedactorLogEntry per la redazione. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getResult()](#getResult--) | Ottiene il risultato, restituito da |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | Ottiene il riferimento alla redazione e le sue opzioni. |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


Inizializza una nuova istanza della classe RedactorLogEntry per la redazione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Riferimento alla redazione |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | Risultato della redazione, segnalato dal gestore del formato |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


Ottiene il risultato, restituito da
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


Ottiene il riferimento alla redazione e le sue opzioni.


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

