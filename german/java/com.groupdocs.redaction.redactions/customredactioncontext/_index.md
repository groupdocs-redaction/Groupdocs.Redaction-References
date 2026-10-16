---
title: "CustomRedactionContext"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Eingabedaten bereit für ."
type: docs
weight: 13
url: /de/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

Stellt Eingabedaten bereit für [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Liefert die Seitenzahl des übereinstimmenden Fragments, falls verfügbar. |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | Setzt die Seitenzahl des übereinstimmenden Fragments. |
|
|  | [getText()](#getText--) | Liefert den für die Redaktion übereinstimmenden Text. |
|
|  | [setText(String value)](#setText-java.lang.String-) | Setzt den für die Redaktion übereinstimmenden Text. |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


Liefert die Seitenzahl des übereinstimmenden Fragments, falls verfügbar.


**Returns:**
int - Die Seitenzahl, oder ein formatabhängiger Wert, wenn die Seite nicht bekannt ist.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


Setzt die Seitenzahl des übereinstimmenden Fragments.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die Seitenzahl. |
|

### getText() {#getText--}
```
public final String getText()
```


Liefert den für die Redaktion übereinstimmenden Text.


**Returns:**
java.lang.String - Der übereinstimmende Text.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Setzt den für die Redaktion übereinstimmenden Text.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Der übereinstimmende Text. |
|

