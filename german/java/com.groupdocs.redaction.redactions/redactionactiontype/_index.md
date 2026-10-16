---
title: "RedactionActionType"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Aktionen dar, die zur Durchführung einer Redaktion ausgeführt werden können."
type: docs
weight: 37
url: /de/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

Stellt Aktionen dar, die zur Durchführung einer Redaktion ausgeführt werden können.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [Replacement](#Replacement) | Redigierter Text wurde durch einen anderen ersetzt oder mit einem Block überdeckt. |
|
|  | [Cleanup](#Cleanup) | Daten wurden entfernt, aber ein leeres Objekt bleibt im Dokument erhalten. |
|
|  | [Deletion](#Deletion) | Daten und zugehörige Strukturen wurden aus dem Dokument entfernt. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


Redigierter Text wurde durch einen anderen ersetzt oder mit einem Block überdeckt.


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


Daten wurden entfernt, aber ein leeres Objekt bleibt im Dokument erhalten.


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


Daten und zugehörige Strukturen wurden aus dem Dokument entfernt.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
