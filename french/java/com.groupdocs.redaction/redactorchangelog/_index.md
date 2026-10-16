---
title: "RedactorChangeLog"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente les résultats pour une liste de rédactions passées à la méthode Apply de la classe Redactor."
type: docs
weight: 17
url: /fr/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Représente les résultats pour une liste de rédactions, passées à la méthode Apply() de
Redactor
classe.

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | Initialise une nouvelle instance de la classe RedactorChangeLog. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getStatus()](#getStatus--) | Obtient l'état final de toutes les rédactions appliquées. |
|
|  | [getRedactionLog()](#getRedactionLog--) | Obtient la liste de |
RedactorLogEntry
instances.
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


Initialise une nouvelle instance de la classe RedactorChangeLog.


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Obtient l'état final de toutes les rédactions appliquées.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


Obtient la liste de
RedactorLogEntry
instances.


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - La liste des instances de RedactorLogEntry.

