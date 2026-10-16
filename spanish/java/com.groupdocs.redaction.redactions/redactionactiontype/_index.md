---
title: "RedactionActionType"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa acciones que pueden tomarse para realizar la redacción."
type: docs
weight: 37
url: /es/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

Representa acciones que pueden tomarse para realizar la redacción.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [Replacement](#Replacement) | El texto redactado fue reemplazado por otro o cubierto con un bloque. |
|
|  | [Cleanup](#Cleanup) | Los datos fueron eliminados, pero un objeto vacío permanece en el documento. |
|
|  | [Deletion](#Deletion) | Los datos y las estructuras relacionadas fueron eliminados del documento. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


El texto redactado fue reemplazado por otro o cubierto con un bloque.


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


Los datos fueron eliminados, pero un objeto vacío permanece en el documento.


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


Los datos y las estructuras relacionadas fueron eliminados del documento.


### values() {#values--}
```
public static RedactionActionType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.RedactionActionType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionActionType valueOf(String name)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
