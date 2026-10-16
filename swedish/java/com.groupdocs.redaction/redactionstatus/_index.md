---
title: "RedactionStatus"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en raderingsslutförandestatus."
type: docs
weight: 20
url: /sv/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

Representerar en raderingsslutförandestatus.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [Applied](#Applied) | Redigering utfördes helt och framgångsrikt. |
|
|  | [PartiallyApplied](#PartiallyApplied) | Redigering tillämpades endast på en del av dess matchningar. |
|
|  | [Skipped](#Skipped) | Redigering hoppades över (inte tillämpad). |
|
|  | [Failed](#Failed) | Redigering misslyckades med undantag. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


Redigering utfördes helt och framgångsrikt.


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


Redigering tillämpades endast på en del av dess matchningar.


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


Redigering hoppades över (inte tillämpad).


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


Redigering misslyckades med undantag.


### values() {#values--}
```
public static RedactionStatus[] values()
```




**Returns:**
com.groupdocs.redaction.RedactionStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionStatus valueOf(String name)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
