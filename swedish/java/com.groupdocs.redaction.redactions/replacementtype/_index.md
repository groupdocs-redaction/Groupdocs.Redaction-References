---
title: "ReplacementType"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en typ av ersättning för den matchade texten."
type: docs
weight: 38
url: /sv/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

Representerar en typ av ersättning för den matchade texten.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | Ersätter matchande text med en annan sträng, t.ex. |
|
|  | [DrawBox](#DrawBox) | Ritar en rektangel i en specifik färg (Svart som standard) istället för redigerad text. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


Ersätter matchande text med en annan sträng, t.ex. undantagskod.


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


Ritar en rektangel i en specifik färg (Svart som standard) istället för redigerad text.


### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
