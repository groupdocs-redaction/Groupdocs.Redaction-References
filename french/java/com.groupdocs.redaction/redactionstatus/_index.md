---
title: "RedactionStatus"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente un statut d'achèvement de la rédaction."
type: docs
weight: 20
url: /fr/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

Représente un statut d'achèvement de la rédaction.

## Champs

| Champ | Description |
| --- | --- |
|  | [Applied](#Applied) | La rédaction a été appliquée entièrement et avec succès. |
|
|  | [PartiallyApplied](#PartiallyApplied) | La rédaction a été appliquée uniquement à une partie de ses correspondances. |
|
|  | [Skipped](#Skipped) | La rédaction a été ignorée (non appliquée). |
|
|  | [Failed](#Failed) | La rédaction a échoué avec une exception. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


La rédaction a été appliquée entièrement et avec succès.


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


La rédaction a été appliquée uniquement à une partie de ses correspondances.


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


La rédaction a été ignorée (non appliquée).


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


La rédaction a échoué avec une exception.


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
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
