---
title: "CustomRedactionResult"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar ett resultat som returneras av ."
type: docs
weight: 14
url: /sv/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

Representerar ett resultat som returneras av [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getApply()](#getApply--) | Hämtar ett värde som indikerar om ersättningen ska tillämpas. |
|
|  | [setApply(boolean value)](#setApply-boolean-) | Ställer in ett värde som indikerar om ersättningen ska tillämpas. |
|
|  | [getText()](#getText--) | Hämtar ersättningstexten som används när #getApply().getApply() är |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | Ställer in ersättningstexten som används när #getApply().getApply() är |
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


Hämtar ett värde som indikerar om ersättningen ska tillämpas.


**Returns:**
boolean -  true  för att ersätta den matchade texten med #getText().getText(); annars,  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


Ställer in ett värde som indikerar om ersättningen ska tillämpas.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | true  för att tillämpa ersättningen; annars,  false . |
|

### getText() {#getText--}
```
public final String getText()
```


Hämtar ersättningstexten som används när #getApply().getApply() är
true
.


**Returns:**
java.lang.String - Ersättningstexten.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Ställer in ersättningstexten som används när #getApply().getApply() är
true
.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Ersättningstexten. |
|

