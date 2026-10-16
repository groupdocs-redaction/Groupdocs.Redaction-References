---
title: "WordProcessingComplianceLevel"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "OOXML‑Konformitätsstufen für Textverarbeitungsdokumente."
type: docs
weight: 22
url: /de/java/com.groupdocs.redaction.options/wordprocessingcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum WordProcessingComplianceLevel extends Enum<WordProcessingComplianceLevel>
```

OOXML-Konformitätsstufen für Textverarbeitungsdokumente. Strict kann nur auf Transitional herabgestuft werden, nicht auf Ecma.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [Ecma](#Ecma) | ECMA-376 1. Auflage, 2006. |
|
|  | [Transitional](#Transitional) | ISO/IEC 29500:2008 Übergangs. |
|
|  | [Strict](#Strict) | ISO/IEC 29500:2008 Strikt. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ecma {#Ecma}
```
public static final WordProcessingComplianceLevel Ecma
```


ECMA-376 1. Auflage, 2006.


### Transitional {#Transitional}
```
public static final WordProcessingComplianceLevel Transitional
```


ISO/IEC 29500:2008 Übergangs.


### Strict {#Strict}
```
public static final WordProcessingComplianceLevel Strict
```


ISO/IEC 29500:2008 Strikt.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
