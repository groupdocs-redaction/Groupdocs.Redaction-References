---
title: "WordprocessingSaveOptions"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Opzioni di salvataggio per l'elaborazione testi."
type: docs
weight: 15
url: /it/java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

Opzioni di salvataggio per l'elaborazione testi.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getOoxmlCompliance()](#getOoxmlCompliance--) | Conformità OOXML da applicare al salvataggio. |
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


Conformità OOXML da applicare al salvataggio.  null  mantiene il livello originale del documento. Strict non può essere salvato come Ecma direttamente; usa prima Transitional.


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

