---
title: "RedactionStatus"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta lo stato di completamento della redazione."
type: docs
weight: 20
url: /it/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

Rappresenta lo stato di completamento della redazione.

## Campi

| Campo | Descrizione |
| --- | --- |
|  | [Applied](#Applied) | La redazione è stata applicata completamente e con successo. |
|
|  | [PartiallyApplied](#PartiallyApplied) | La redazione è stata applicata solo a una parte delle sue corrispondenze. |
|
|  | [Skipped](#Skipped) | La redazione è stata saltata (non applicata). |
|
|  | [Failed](#Failed) | La redazione è fallita con eccezione. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


La redazione è stata applicata completamente e con successo.


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


La redazione è stata applicata solo a una parte delle sue corrispondenze.


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


La redazione è stata saltata (non applicata).


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


La redazione è fallita con eccezione.


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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
