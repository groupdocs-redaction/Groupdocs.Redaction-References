---
title: "WordprocessingSaveOptions"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Options d'enregistrement du traitement de texte."
type: docs
weight: 15
url: /fr/java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

Options d'enregistrement du traitement de texte.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getOoxmlCompliance()](#getOoxmlCompliance--) | Conformité OOXML à appliquer lors de l'enregistrement. |
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


Conformité OOXML à appliquer lors de l'enregistrement.  null  conserve le niveau de document original. Strict ne peut pas être enregistré directement en tant qu'Ecma ; utilisez Transitional d'abord.


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

