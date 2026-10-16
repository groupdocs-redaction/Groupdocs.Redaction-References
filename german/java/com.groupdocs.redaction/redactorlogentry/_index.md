---
title: "RedactorLogEntry"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Ergebnisse der Anwendung von Redaktionen dar."
type: docs
weight: 18
url: /de/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

Stellt Ergebnisse der Anwendung von Redaktionen dar.

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | Initialisiert eine neue Instanz der RedactorLogEntry-Klasse für die Redaktion. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getResult()](#getResult--) | Liefert das Ergebnis, zurückgegeben von |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | Liefert die Referenz zur Redaktion und deren Optionen. |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


Initialisiert eine neue Instanz der RedactorLogEntry-Klasse für die Redaktion.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Referenz zur Redaktion |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | Redaktionsergebnis, gemeldet vom Format-Handler |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


Liefert das Ergebnis, zurückgegeben von
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


Liefert die Referenz zur Redaktion und deren Optionen.


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

