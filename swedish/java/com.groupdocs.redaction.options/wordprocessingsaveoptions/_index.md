---
title: "WordprocessingSaveOptions"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Sparaalternativ för ordbehandling."
type: docs
weight: 15
url: /sv/java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

Sparaalternativ för ordbehandling.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getOoxmlCompliance()](#getOoxmlCompliance--) | OOXML-efterlevnad att tillämpa vid sparande. |
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


OOXML-efterlevnad att tillämpa vid sparande.  null  behåller den ursprungliga dokumentnivån. Strict kan inte sparas som Ecma direkt; använd Transitional först.


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

