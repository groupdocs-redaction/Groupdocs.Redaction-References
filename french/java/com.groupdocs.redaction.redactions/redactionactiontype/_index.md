---
title: "RedactionActionType"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente les actions qui peuvent être effectuées pour réaliser la rédaction."
type: docs
weight: 37
url: /fr/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

Représente les actions qui peuvent être effectuées pour réaliser la rédaction.

## Champs

| Champ | Description |
| --- | --- |
|  | [Replacement](#Replacement) | Le texte censuré a été remplacé par un autre ou couvert par un bloc. |
|
|  | [Cleanup](#Cleanup) | Les données ont été supprimées, mais un objet vide reste dans le document. |
|
|  | [Deletion](#Deletion) | Les données et les structures associées ont été supprimées du document. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


Le texte censuré a été remplacé par un autre ou couvert par un bloc.


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


Les données ont été supprimées, mais un objet vide reste dans le document.


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


Les données et les structures associées ont été supprimées du document.


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
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
