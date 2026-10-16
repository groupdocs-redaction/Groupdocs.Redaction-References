---
title: "CustomRedactionContext"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Levert invoergegevens voor ."
type: docs
weight: 13
url: /nl/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

Levert invoergegevens voor [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Haalt het paginanummer op van het overeenkomende fragment, indien beschikbaar. |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | Stelt het paginanummer in van het overeenkomende fragment. |
|
|  | [getText()](#getText--) | Haalt de tekst op die overeenkomt voor redactie. |
|
|  | [setText(String value)](#setText-java.lang.String-) | Stelt de tekst in die overeenkomt voor redactie. |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


Haalt het paginanummer op van het overeenkomende fragment, indien beschikbaar.


**Returns:**
int - Het paginanummer, of een formaat‑specifieke waarde als de pagina onbekend is.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


Stelt het paginanummer in van het overeenkomende fragment.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het paginanummer. |
|

### getText() {#getText--}
```
public final String getText()
```


Haalt de tekst op die overeenkomt voor redactie.


**Returns:**
java.lang.String - De overeenkomende tekst.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Stelt de tekst in die overeenkomt voor redactie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | De overeenkomende tekst. |
|

