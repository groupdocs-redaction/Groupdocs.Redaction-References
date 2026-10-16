---
title: "RedactionResult"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta un risultato dell'operazione di redazione."
type: docs
weight: 15
url: /it/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

Rappresenta un risultato dell'operazione di redazione.

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getStatus()](#getStatus--) | Restituisce lo stato di esecuzione. |
|
|  | [getErrorMessage()](#getErrorMessage--) | Restituisce il messaggio di errore per la diagnostica. |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | Inizializza una nuova istanza della classe RedactionResult con stato Skipped. |
|
|  | [partial(String description)](#partial-java.lang.String-) | Inizializza una nuova istanza della classe RedactionResult con stato PartiallyApplied. |
|
|  | [failed(String description)](#failed-java.lang.String-) | Inizializza una nuova istanza della classe RedactionResult con stato Failed. |
|
|  | [successful()](#successful--) | Inizializza una nuova istanza della classe RedactionResult con stato Applied (riuscito). |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Restituisce lo stato di esecuzione.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


Restituisce il messaggio di errore per la diagnostica.


**Returns:**
java.lang.String - Il messaggio di errore per la diagnostica.

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


Inizializza una nuova istanza della classe RedactionResult con stato Skipped.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | descrizione | java.lang.String | Motivo per cui l'operazione è stata saltata |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


Inizializza una nuova istanza della classe RedactionResult con stato PartiallyApplied.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | descrizione | java.lang.String | Motivo per cui l'operazione non è stata completamente applicata |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


Inizializza una nuova istanza della classe RedactionResult con stato Failed.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | descrizione | java.lang.String | Dettagli di errore o eccezione |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


Inizializza una nuova istanza della classe RedactionResult con stato Applied (riuscito).


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

