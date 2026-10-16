---
title: "CustomRedactionResult"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt ein Ergebnis dar, das von . zurückgegeben wird."
type: docs
weight: 14
url: /de/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

Stellt ein Ergebnis dar, das von [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) zurückgegeben wird.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getApply()](#getApply--) | Liefert einen Wert, der angibt, ob die Ersetzung angewendet werden soll. |
|
|  | [setApply(boolean value)](#setApply-boolean-) | Setzt einen Wert, der angibt, ob die Ersetzung angewendet werden soll. |
|
|  | [getText()](#getText--) | Liefert den Ersetzungstext, der verwendet wird, wenn #getApply().getApply() ist |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | Setzt den Ersetzungstext, der verwendet wird, wenn #getApply().getApply() ist |
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


Liefert einen Wert, der angibt, ob die Ersetzung angewendet werden soll.


**Returns:**
boolean -  true  um den gefundenen Text mit #getText().getText() zu ersetzen; andernfalls  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


Setzt einen Wert, der angibt, ob die Ersetzung angewendet werden soll.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | true  um die Ersetzung anzuwenden; andernfalls  false . |
|

### getText() {#getText--}
```
public final String getText()
```


Liefert den Ersetzungstext, der verwendet wird, wenn #getApply().getApply() ist
true
.


**Returns:**
java.lang.String - Der Ersetzungstext.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Setzt den Ersetzungstext, der verwendet wird, wenn #getApply().getApply() ist
true
.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Der Ersetzungstext. |
|

