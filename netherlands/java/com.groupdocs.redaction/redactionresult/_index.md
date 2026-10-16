---
title: "RedactionResult"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een resultaat van de redactiebewerking voor."
type: docs
weight: 15
url: /nl/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

Stelt een resultaat van de redactiebewerking voor.

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getStatus()](#getStatus--) | Haalt de uitvoeringsstatus op. |
|
|  | [getErrorMessage()](#getErrorMessage--) | Haalt het foutbericht op voor diagnostiek. |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | Initialiseert een nieuw exemplaar van de RedactionResult-klasse met de status Skipped. |
|
|  | [partial(String description)](#partial-java.lang.String-) | Initialiseert een nieuw exemplaar van de RedactionResult-klasse met de status PartiallyApplied. |
|
|  | [failed(String description)](#failed-java.lang.String-) | Initialiseert een nieuw exemplaar van de RedactionResult-klasse met de status Failed. |
|
|  | [successful()](#successful--) | Initialiseert een nieuw exemplaar van de RedactionResult-klasse met de status Applied (succesvol). |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Haalt de uitvoeringsstatus op.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


Haalt het foutbericht op voor diagnostiek.


**Returns:**
java.lang.String - Het foutbericht voor diagnostiek.

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


Initialiseert een nieuw exemplaar van de RedactionResult-klasse met de status Skipped.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | beschrijving | java.lang.String | Reden waarom de bewerking werd overgeslagen |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


Initialiseert een nieuw exemplaar van de RedactionResult-klasse met de status PartiallyApplied.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | beschrijving | java.lang.String | Reden waarom de bewerking niet volledig werd toegepast |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


Initialiseert een nieuw exemplaar van de RedactionResult-klasse met de status Failed.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | beschrijving | java.lang.String | Fout- of exceptiegegevens |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


Initialiseert een nieuw exemplaar van de RedactionResult-klasse met de status Applied (succesvol).


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

