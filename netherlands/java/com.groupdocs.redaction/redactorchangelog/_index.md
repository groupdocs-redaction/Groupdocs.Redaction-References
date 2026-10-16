---
title: "RedactorChangeLog"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt resultaten voor een lijst van redactionele bewerkingen die zijn doorgegeven aan de Apply-methode van de Redactor-klasse."
type: docs
weight: 17
url: /nl/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Stelt resultaten voor een lijst van redactionele bewerkingen, doorgegeven aan de Apply()-methode van
Redactor
klasse.

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | Initialiseert een nieuw exemplaar van de RedactorChangeLog-klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getStatus()](#getStatus--) | Haalt de uiteindelijke status op van alle toegepaste redactionele bewerkingen. |
|
|  | [getRedactionLog()](#getRedactionLog--) | Haalt de lijst op van |
RedactorLogEntry
instances.
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


Initialiseert een nieuw exemplaar van de RedactorChangeLog-klasse.


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Haalt de uiteindelijke status op van alle toegepaste redactionele bewerkingen.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


Haalt de lijst op van
RedactorLogEntry
instances.


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - De lijst met RedactorLogEntry instanties.

