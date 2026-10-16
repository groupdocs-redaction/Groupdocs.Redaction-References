---
title: "RedactionResult"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa un resultado de la operación de redacción."
type: docs
weight: 15
url: /es/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

Representa un resultado de la operación de redacción.

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Métodos

| Método | Descripción |
| --- | --- |
|  | [getStatus()](#getStatus--) | Obtiene el estado de ejecución. |
|
|  | [getErrorMessage()](#getErrorMessage--) | Obtiene el mensaje de error para diagnóstico. |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | Inicializa una nueva instancia de la clase RedactionResult con el estado Skipped. |
|
|  | [partial(String description)](#partial-java.lang.String-) | Inicializa una nueva instancia de la clase RedactionResult con el estado PartiallyApplied. |
|
|  | [failed(String description)](#failed-java.lang.String-) | Inicializa una nueva instancia de la clase RedactionResult con el estado Failed. |
|
|  | [successful()](#successful--) | Inicializa una nueva instancia de la clase RedactionResult con el estado Applied (exitoso). |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Obtiene el estado de ejecución.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


Obtiene el mensaje de error para diagnóstico.


**Returns:**
java.lang.String - El mensaje de error para diagnóstico.

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


Inicializa una nueva instancia de la clase RedactionResult con el estado Skipped.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | descripción | java.lang.String | Razón por la que la operación fue omitida |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


Inicializa una nueva instancia de la clase RedactionResult con el estado PartiallyApplied.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | descripción | java.lang.String | Razón por la que la operación no se aplicó completamente |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


Inicializa una nueva instancia de la clase RedactionResult con el estado Failed.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | descripción | java.lang.String | Detalles de falla o excepción |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


Inicializa una nueva instancia de la clase RedactionResult con el estado Applied (exitoso).


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

