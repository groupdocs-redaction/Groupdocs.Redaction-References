---
title: "CustomRedactionContext"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Tillhandahåller indata för ."
type: docs
weight: 13
url: /sv/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

Tillhandahåller indata för [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Hämtar sidnumret för det matchade fragmentet, när det är tillgängligt. |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | Ställer in sidnumret för det matchade fragmentet. |
|
|  | [getText()](#getText--) | Hämtar den text som matchas för redigering. |
|
|  | [setText(String value)](#setText-java.lang.String-) | Ställer in den text som matchas för redigering. |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


Hämtar sidnumret för det matchade fragmentet, när det är tillgängligt.


**Returns:**
int - Sidnumret, eller ett format-specifikt värde om sidan inte är känd.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


Ställer in sidnumret för det matchade fragmentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Sidnumret. |
|

### getText() {#getText--}
```
public final String getText()
```


Hämtar den text som matchas för redigering.


**Returns:**
java.lang.String - Den matchade texten.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Ställer in den text som matchas för redigering.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Den matchade texten. |
|

