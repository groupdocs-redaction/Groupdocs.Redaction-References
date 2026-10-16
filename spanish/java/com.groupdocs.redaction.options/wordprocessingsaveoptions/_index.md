---
title: "WordprocessingSaveOptions"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Opciones de guardado de procesamiento de texto."
type: docs
weight: 15
url: /es/java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

Opciones de guardado de procesamiento de texto.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getOoxmlCompliance()](#getOoxmlCompliance--) | Cumplimiento OOXML a aplicar al guardar. |
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


Cumplimiento OOXML a aplicar al guardar.  null  mantiene el nivel original del documento. Strict no puede guardarse como Ecma directamente; use Transitional primero.


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

