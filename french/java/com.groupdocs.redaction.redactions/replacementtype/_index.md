---
title: "ReplacementType"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente un type de remplacement pour le texte correspondant."
type: docs
weight: 38
url: /fr/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

Représente un type de remplacement pour le texte correspondant.

## Champs

| Champ | Description |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | Remplace le texte correspondant par une autre chaîne, p. ex. |
|
|  | [DrawBox](#DrawBox) | Dessine un rectangle d'une couleur spécifique (Noir par défaut) à la place du texte censuré. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


Remplace le texte correspondant par une autre chaîne, p. ex. code d'exemption.


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


Dessine un rectangle d'une couleur spécifique (Noir par défaut) à la place du texte censuré.


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
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
