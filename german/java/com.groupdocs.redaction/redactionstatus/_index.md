---
title: "RedactionStatus"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt einen Redaktionsabschlussstatus dar."
type: docs
weight: 20
url: /de/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

Stellt einen Redaktionsabschlussstatus dar.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [Applied](#Applied) | Redaction wurde vollständig und erfolgreich angewendet. |
|
|  | [PartiallyApplied](#PartiallyApplied) | Redaction wurde nur auf einen Teil ihrer Treffer angewendet. |
|
|  | [Skipped](#Skipped) | Redaktion wurde übersprungen (nicht angewendet). |
|
|  | [Failed](#Failed) | Redaktion ist mit einer Ausnahme fehlgeschlagen. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


Redaction wurde vollständig und erfolgreich angewendet.


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


Redaction wurde nur auf einen Teil ihrer Treffer angewendet.


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


Redaktion wurde übersprungen (nicht angewendet).


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


Redaktion ist mit einer Ausnahme fehlgeschlagen.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
