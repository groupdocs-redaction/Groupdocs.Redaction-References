---
title: "RedactionActionType"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar åtgärder som kan vidtas för att utföra redigering."
type: docs
weight: 37
url: /sv/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

Representerar åtgärder som kan vidtas för att utföra redigering.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [Replacement](#Replacement) | Redigerad text ersattes med en annan eller täcktes med ett block. |
|
|  | [Cleanup](#Cleanup) | Data togs bort, men ett tomt objekt finns kvar i dokumentet. |
|
|  | [Deletion](#Deletion) | Data och relaterade strukturer togs bort från dokumentet. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


Redigerad text ersattes med en annan eller täcktes med ett block.


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


Data togs bort, men ett tomt objekt finns kvar i dokumentet.


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


Data och relaterade strukturer togs bort från dokumentet.


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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
