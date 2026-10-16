---
title: "RedactionStatus"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een status van voltooiing van de redactiewerkzaamheden voor."
type: docs
weight: 20
url: /nl/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

Stelt een status van voltooiing van de redactiewerkzaamheden voor.

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [Applied](#Applied) | Redactie was volledig en succesvol toegepast. |
|
|  | [PartiallyApplied](#PartiallyApplied) | Redactie werd alleen toegepast op een deel van de overeenkomsten. |
|
|  | [Skipped](#Skipped) | Redactie werd overgeslagen (niet toegepast). |
|
|  | [Failed](#Failed) | Redactie is mislukt met een uitzondering. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


Redactie was volledig en succesvol toegepast.


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


Redactie werd alleen toegepast op een deel van de overeenkomsten.


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


Redactie werd overgeslagen (niet toegepast).


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


Redactie is mislukt met een uitzondering.


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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
