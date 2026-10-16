---
title: "RedactionStatus"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa un estado de finalización de la redacción."
type: docs
weight: 20
url: /es/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

Representa un estado de finalización de la redacción.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [Applied](#Applied) | La redacción se aplicó completa y exitosamente. |
|
|  | [PartiallyApplied](#PartiallyApplied) | La redacción se aplicó solo a una parte de sus coincidencias. |
|
|  | [Skipped](#Skipped) | La redacción fue omitida (no aplicada). |
|
|  | [Failed](#Failed) | La redacción falló con excepción. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


La redacción se aplicó completa y exitosamente.


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


La redacción se aplicó solo a una parte de sus coincidencias.


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


La redacción fue omitida (no aplicada).


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


La redacción falló con excepción.


### values() {#values--}
```
public static RedactionStatus[] values()
```




**Returns:**
com.groupdocs.redaction.RedactionStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionStatus valueOf(String name)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
