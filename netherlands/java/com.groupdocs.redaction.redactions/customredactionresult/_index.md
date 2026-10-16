---
title: "CustomRedactionResult"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een resultaat voor dat wordt geretourneerd door ."
type: docs
weight: 14
url: /nl/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

Stelt een resultaat voor dat wordt geretourneerd door [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getApply()](#getApply--) | Haalt een waarde op die aangeeft of de vervanging moet worden toegepast. |
|
|  | [setApply(boolean value)](#setApply-boolean-) | Stelt een waarde in die aangeeft of de vervanging moet worden toegepast. |
|
|  | [getText()](#getText--) | Haalt de vervangende tekst op die wordt gebruikt wanneer #getApply().getApply() is |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | Stelt de vervangende tekst in die wordt gebruikt wanneer #getApply().getApply() is |
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


Haalt een waarde op die aangeeft of de vervanging moet worden toegepast.


**Returns:**
boolean -  true  om de overeenkomende tekst te vervangen door #getText().getText(); anders,  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


Stelt een waarde in die aangeeft of de vervanging moet worden toegepast.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | true  om de vervanging toe te passen; anders,  false . |
|

### getText() {#getText--}
```
public final String getText()
```


Haalt de vervangende tekst op die wordt gebruikt wanneer #getApply().getApply() is
true
.


**Returns:**
java.lang.String - De vervangende tekst.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Stelt de vervangende tekst in die wordt gebruikt wanneer #getApply().getApply() is
true
.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | De vervangende tekst. |
|

