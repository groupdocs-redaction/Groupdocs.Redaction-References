---
title: "RedactorLogEntry"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa resultados de la aplicación de la redacción."
type: docs
weight: 18
url: /es/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

Representa resultados de la aplicación de la redacción.

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | Inicializa una nueva instancia de la clase RedactorLogEntry para la redacción. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getResult()](#getResult--) | Obtiene el resultado, devuelto por |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | Obtiene la referencia a la redacción y sus opciones. |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


Inicializa una nueva instancia de la clase RedactorLogEntry para la redacción.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Referencia a la redacción. |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | Resultado de la redacción, reportado por el controlador de formato. |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


Obtiene el resultado, devuelto por
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


Obtiene la referencia a la redacción y sus opciones.


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

