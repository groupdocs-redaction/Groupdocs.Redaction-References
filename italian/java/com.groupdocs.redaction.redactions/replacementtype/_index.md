---
title: "ReplacementType"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta un tipo di sostituzione per il testo corrispondente."
type: docs
weight: 38
url: /it/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

Rappresenta un tipo di sostituzione per il testo corrispondente.

## Campi

| Campo | Descrizione |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | Sostituisce il testo corrispondente con un'altra stringa, per es. |
|
|  | [DrawBox](#DrawBox) | Disegna un rettangolo di colore specifico (Nero per impostazione predefinita) al posto del testo redatto. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


Sostituisce il testo corrispondente con un'altra stringa, per es. codice di esenzione.


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


Disegna un rettangolo di colore specifico (Nero per impostazione predefinita) al posto del testo redatto.


### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
