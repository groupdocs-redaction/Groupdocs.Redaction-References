---
title: "RedactorChangeLog"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Ergebnisse für eine Liste von Redaktionen dar, die an die Apply-Methode der Redactor-Klasse übergeben wurden."
type: docs
weight: 17
url: /de/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Stellt Ergebnisse für eine Liste von Redaktionen dar, die an die Apply()-Methode von
Redactor
Klasse.

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | Initialisiert eine neue Instanz der RedactorChangeLog-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getStatus()](#getStatus--) | Ermittelt den endgültigen Status aller angewendeten Redaktionen. |
|
|  | [getRedactionLog()](#getRedactionLog--) | Ermittelt die Liste von |
RedactorLogEntry
Instanzen.
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


Initialisiert eine neue Instanz der RedactorChangeLog-Klasse.


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Ermittelt den endgültigen Status aller angewendeten Redaktionen.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


Ermittelt die Liste von
RedactorLogEntry
Instanzen.


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - Die Liste der  RedactorLogEntry  Instanzen.

