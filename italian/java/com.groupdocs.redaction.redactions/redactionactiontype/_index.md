---
title: "RedactionActionType"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta le azioni che possono essere eseguite per effettuare la redazione."
type: docs
weight: 37
url: /it/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

Rappresenta le azioni che possono essere eseguite per effettuare la redazione.

## Campi

| Campo | Descrizione |
| --- | --- |
|  | [Replacement](#Replacement) | Il testo redatto è stato sostituito con un altro o coperto da un blocco. |
|
|  | [Cleanup](#Cleanup) | I dati sono stati rimossi, ma un oggetto vuoto rimane nel documento. |
|
|  | [Deletion](#Deletion) | I dati e le strutture correlate sono stati rimossi dal documento. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


Il testo redatto è stato sostituito con un altro o coperto da un blocco.


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


I dati sono stati rimossi, ma un oggetto vuoto rimane nel documento.


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


I dati e le strutture correlate sono stati rimossi dal documento.


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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
