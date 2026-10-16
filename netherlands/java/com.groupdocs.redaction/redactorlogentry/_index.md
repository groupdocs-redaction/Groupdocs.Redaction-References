---
title: "RedactorLogEntry"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt resultaten voor van het toepassen van redacties."
type: docs
weight: 18
url: /nl/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

Stelt resultaten voor van het toepassen van redacties.

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | Initialiseert een nieuw exemplaar van de RedactorLogEntry-klasse voor redaction. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getResult()](#getResult--) | Haalt het resultaat op, geretourneerd door |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | Haalt de referentie naar redactie en de opties op. |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


Initialiseert een nieuw exemplaar van de RedactorLogEntry-klasse voor redaction.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Referentie naar redactie |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | Redactieresultaat, gerapporteerd door de formaathandler |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


Haalt het resultaat op, geretourneerd door
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


Haalt de referentie naar redactie en de opties op.


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

