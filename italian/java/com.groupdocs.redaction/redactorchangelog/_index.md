---
title: "RedactorChangeLog"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta i risultati per un elenco di redazioni passato al metodo Apply della classe Redactor."
type: docs
weight: 17
url: /it/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Rappresenta i risultati per un elenco di redazioni, passato al metodo Apply() di
Redactor
classe.

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | Inizializza una nuova istanza della classe RedactorChangeLog. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getStatus()](#getStatus--) | Ottiene lo stato finale di tutte le redazioni applicate. |
|
|  | [getRedactionLog()](#getRedactionLog--) | Ottiene l'elenco di |
RedactorLogEntry
istanze.
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


Inizializza una nuova istanza della classe RedactorChangeLog.


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Ottiene lo stato finale di tutte le redazioni applicate.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


Ottiene l'elenco di
RedactorLogEntry
istanze.


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - L'elenco delle istanze di RedactorLogEntry.

