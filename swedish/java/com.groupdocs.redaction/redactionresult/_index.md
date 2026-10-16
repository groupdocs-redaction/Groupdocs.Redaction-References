---
title: "RedactionResult"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar ett resultat av raderingsoperationen."
type: docs
weight: 15
url: /sv/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

Representerar ett resultat av raderingsoperationen.

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getStatus()](#getStatus--) | Hämtar exekveringsstatusen. |
|
|  | [getErrorMessage()](#getErrorMessage--) | Hämtar felmeddelandet för diagnostik. |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | Initierar en ny instans av klassen RedactionResult med statusen Skipped. |
|
|  | [partial(String description)](#partial-java.lang.String-) | Initierar en ny instans av klassen RedactionResult med statusen PartiallyApplied. |
|
|  | [failed(String description)](#failed-java.lang.String-) | Initierar en ny instans av klassen RedactionResult med statusen Failed. |
|
|  | [successful()](#successful--) | Initierar en ny instans av klassen RedactionResult med statusen Applied (framgångsrik). |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Hämtar exekveringsstatusen.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


Hämtar felmeddelandet för diagnostik.


**Returns:**
java.lang.String – Felmeddelandet för diagnostik.

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


Initierar en ny instans av klassen RedactionResult med statusen Skipped.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | beskrivning | java.lang.String | Orsak till att operationen hoppades över |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


Initierar en ny instans av klassen RedactionResult med statusen PartiallyApplied.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | beskrivning | java.lang.String | Orsak till att operationen inte tillämpades fullt ut |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


Initierar en ny instans av klassen RedactionResult med statusen Failed.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | beskrivning | java.lang.String | Detaljer om fel eller undantag |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


Initierar en ny instans av klassen RedactionResult med statusen Applied (framgångsrik).


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

