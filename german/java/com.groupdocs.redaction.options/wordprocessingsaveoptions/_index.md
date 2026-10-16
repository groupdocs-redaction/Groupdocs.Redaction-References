---
title: "WordprocessingSaveOptions"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Speicheroptionen für die Textverarbeitung."
type: docs
weight: 15
url: /de/java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

Speicheroptionen für die Textverarbeitung.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getOoxmlCompliance()](#getOoxmlCompliance--) | OOXML-Konformität, die beim Speichern angewendet wird. |
|
| [setOoxmlCompliance(WordProcessingComplianceLevel value)](#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-) |  |
### WordprocessingSaveOptions() {#WordprocessingSaveOptions--}
```
public WordprocessingSaveOptions()
```


### getOoxmlCompliance() {#getOoxmlCompliance--}
```
public final WordProcessingComplianceLevel getOoxmlCompliance()
```


OOXML-Konformität, die beim Speichern angewendet wird.  null  behält die ursprüngliche Dokumentebene bei. Strict kann nicht direkt als Ecma gespeichert werden; zuerst Transitional verwenden.


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

