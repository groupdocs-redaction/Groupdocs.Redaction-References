---
title: "RedactorChangeLog"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar resultat för en lista med redigeringar som skickas till Apply‑metoden i Redactor‑klassen."
type: docs
weight: 17
url: /sv/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Representerar resultat för en lista med redigeringar, som skickas till Apply()-metoden i
Redactor
klass.

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | Initierar en ny instans av RedactorChangeLog‑klassen. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getStatus()](#getStatus--) | Hämtar det slutgiltiga status för alla tillämpade redigeringar. |
|
|  | [getRedactionLog()](#getRedactionLog--) | Hämtar listan över |
RedactorLogEntry
instanser.
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


Initierar en ny instans av RedactorChangeLog‑klassen.


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Hämtar det slutgiltiga status för alla tillämpade redigeringar.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


Hämtar listan över
RedactorLogEntry
instanser.


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - Listan med RedactorLogEntry‑instanser.

