---
title: "RedactionActionType"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Vertegenwoordigt acties die kunnen worden ondernomen om redacties uit te voeren."
type: docs
weight: 37
url: /nl/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

Vertegenwoordigt acties die kunnen worden ondernomen om redacties uit te voeren.

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [Replacement](#Replacement) | Geredacteerde tekst werd vervangen door een andere of bedekt met een blok. |
|
|  | [Cleanup](#Cleanup) | Gegevens werden verwijderd, maar een leeg object blijft in het document. |
|
|  | [Deletion](#Deletion) | Gegevens en gerelateerde structuren werden uit het document verwijderd. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


Geredacteerde tekst werd vervangen door een andere of bedekt met een blok.


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


Gegevens werden verwijderd, maar een leeg object blijft in het document.


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


Gegevens en gerelateerde structuren werden uit het document verwijderd.


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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
