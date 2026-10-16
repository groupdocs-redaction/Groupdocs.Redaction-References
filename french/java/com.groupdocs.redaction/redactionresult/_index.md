---
title: "RedactionResult"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente un résultat de l'opération de rédaction."
type: docs
weight: 15
url: /fr/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

Représente un résultat de l'opération de rédaction.

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getStatus()](#getStatus--) | Obtient l'état d'exécution. |
|
|  | [getErrorMessage()](#getErrorMessage--) | Obtient le message d'erreur pour le diagnostic. |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | Initialise une nouvelle instance de la classe RedactionResult avec l'état Skipped. |
|
|  | [partial(String description)](#partial-java.lang.String-) | Initialise une nouvelle instance de la classe RedactionResult avec l'état PartiallyApplied. |
|
|  | [failed(String description)](#failed-java.lang.String-) | Initialise une nouvelle instance de la classe RedactionResult avec l'état Failed. |
|
|  | [successful()](#successful--) | Initialise une nouvelle instance de la classe RedactionResult avec l'état Applied (réussi). |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Obtient l'état d'exécution.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


Obtient le message d'erreur pour le diagnostic.


**Returns:**
java.lang.String - Le message d'erreur pour le diagnostic.

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


Initialise une nouvelle instance de la classe RedactionResult avec l'état Skipped.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | description | java.lang.String | Raison pour laquelle l'opération a été ignorée |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


Initialise une nouvelle instance de la classe RedactionResult avec l'état PartiallyApplied.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | description | java.lang.String | Raison pour laquelle l'opération n'a pas été entièrement appliquée |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


Initialise une nouvelle instance de la classe RedactionResult avec l'état Failed.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | description | java.lang.String | Détails de l'échec ou de l'exception |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


Initialise une nouvelle instance de la classe RedactionResult avec l'état Applied (réussi).


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

