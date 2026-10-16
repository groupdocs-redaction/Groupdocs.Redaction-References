---
title: "RedactionResult"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt ein Ergebnis der Redaktionsoperation dar."
type: docs
weight: 15
url: /de/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

Stellt ein Ergebnis der Redaktionsoperation dar.

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getStatus()](#getStatus--) | Liest den Ausführungsstatus. |
|
|  | [getErrorMessage()](#getErrorMessage--) | Liest die Fehlermeldung für die Diagnose. |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | Initialisiert eine neue Instanz der Klasse RedactionResult mit dem Status Skipped. |
|
|  | [partial(String description)](#partial-java.lang.String-) | Initialisiert eine neue Instanz der Klasse RedactionResult mit dem Status PartiallyApplied. |
|
|  | [failed(String description)](#failed-java.lang.String-) | Initialisiert eine neue Instanz der Klasse RedactionResult mit dem Status Failed. |
|
|  | [successful()](#successful--) | Initialisiert eine neue Instanz der Klasse RedactionResult mit dem Status Applied (erfolgreich). |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Liest den Ausführungsstatus.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


Liest die Fehlermeldung für die Diagnose.


**Returns:**
java.lang.String - Die Fehlermeldung für die Diagnose.

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


Initialisiert eine neue Instanz der Klasse RedactionResult mit dem Status Skipped.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Beschreibung | java.lang.String | Grund, warum die Operation übersprungen wurde |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


Initialisiert eine neue Instanz der Klasse RedactionResult mit dem Status PartiallyApplied.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Beschreibung | java.lang.String | Grund, warum die Operation nicht vollständig angewendet wurde |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


Initialisiert eine neue Instanz der Klasse RedactionResult mit dem Status Failed.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Beschreibung | java.lang.String | Fehler- oder Ausnahmedetails |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


Initialisiert eine neue Instanz der Klasse RedactionResult mit dem Status Applied (erfolgreich).


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

