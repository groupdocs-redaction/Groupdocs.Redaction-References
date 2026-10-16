---
title: "WordProcessingComplianceLevel"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Niveaux de conformité OOXML pour les documents de traitement de texte."
type: docs
weight: 22
url: /fr/java/com.groupdocs.redaction.options/wordprocessingcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum WordProcessingComplianceLevel extends Enum<WordProcessingComplianceLevel>
```

Niveaux de conformité OOXML pour les documents de traitement de texte. Le mode Strict peut être rétrogradé uniquement vers le mode Transitional, pas vers Ecma.

## Champs

| Champ | Description |
| --- | --- |
|  | [Ecma](#Ecma) | ECMA-376 1re édition, 2006. |
|
|  | [Transitional](#Transitional) | ISO/IEC 29500:2008 Transitional. |
|
|  | [Strict](#Strict) | ISO/IEC 29500:2008 Strict. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ecma {#Ecma}
```
public static final WordProcessingComplianceLevel Ecma
```


ECMA-376 1re édition, 2006.


### Transitional {#Transitional}
```
public static final WordProcessingComplianceLevel Transitional
```


ISO/IEC 29500:2008 Transitional.


### Strict {#Strict}
```
public static final WordProcessingComplianceLevel Strict
```


ISO/IEC 29500:2008 Strict.


### values() {#values--}
```
public static WordProcessingComplianceLevel[] values()
```




**Returns:**
com.groupdocs.redaction.options.WordProcessingComplianceLevel[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static WordProcessingComplianceLevel valueOf(String name)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
