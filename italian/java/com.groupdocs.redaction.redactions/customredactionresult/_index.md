---
title: "CustomRedactionResult"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta un risultato restituito da ."
type: docs
weight: 14
url: /it/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

Rappresenta un risultato restituito da [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getApply()](#getApply--) | Ottiene un valore che indica se la sostituzione deve essere applicata. |
|
|  | [setApply(boolean value)](#setApply-boolean-) | Imposta un valore che indica se la sostituzione deve essere applicata. |
|
|  | [getText()](#getText--) | Ottiene il testo di sostituzione usato quando #getApply().getApply() è |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | Imposta il testo di sostituzione usato quando #getApply().getApply() è |
true
.
|
### CustomRedactionResult() {#CustomRedactionResult--}
```
public CustomRedactionResult()
```


### getApply() {#getApply--}
```
public final boolean getApply()
```


Ottiene un valore che indica se la sostituzione deve essere applicata.


**Returns:**
boolean -  true  per sostituire il testo corrispondente con #getText().getText(); altrimenti,  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


Imposta un valore che indica se la sostituzione deve essere applicata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | true  per applicare la sostituzione; altrimenti,  false . |
|

### getText() {#getText--}
```
public final String getText()
```


Ottiene il testo di sostituzione usato quando #getApply().getApply() è
true
.


**Returns:**
java.lang.String - Il testo di sostituzione.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Imposta il testo di sostituzione usato quando #getApply().getApply() è
true
.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Il testo di sostituzione. |
|

