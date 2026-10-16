---
title: "RedactorLogEntry"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar resultat av att tillämpa radering."
type: docs
weight: 18
url: /sv/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

Representerar resultat av att tillämpa radering.

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | Initierar en ny instans av RedactorLogEntry‑klassen för redigering. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getResult()](#getResult--) | Hämtar resultatet, returnerat av |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | Hämtar referensen till redigering och dess alternativ. |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


Initierar en ny instans av RedactorLogEntry‑klassen för redigering.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Referens till redigering |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | Redigeringsresultat, rapporterat av format‑hanteraren |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


Hämtar resultatet, returnerat av
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


Hämtar referensen till redigering och dess alternativ.


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

