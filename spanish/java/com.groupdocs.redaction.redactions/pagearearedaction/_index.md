---
title: "PageAreaRedaction"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una redacción textual compleja que afecta a imágenes de texto y anotaciones en un área de la página."
type: docs
weight: 23
url: /es/java/com.groupdocs.redaction.redactions/pagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction), [com.groupdocs.redaction.redactions.RegexRedaction](../../com.groupdocs.redaction.redactions/regexredaction)
```
public class PageAreaRedaction extends RegexRedaction
```

Representa una redacción textual compleja que afecta texto, imágenes y anotaciones en un área de la página.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](../https://docs.groupdocs.com/redaction/java/use-page-area-redaction/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Inicializa una nueva instancia de la clase PageAreaRedaction. |
|
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Inicializa una nueva instancia de la clase PageAreaRedaction. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getImageOptions()](#getImageOptions--) | Obtiene el |
RegionReplacementOptions
opciones con parámetros de color y área.
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Aplica la redacción a una instancia de formato dada. |
|
### PageAreaRedaction(Pattern regex, ReplacementOptions options) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options)
```


Inicializa una nueva instancia de la clase PageAreaRedaction.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Expresión regular para buscar y reemplazar |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opciones de reemplazo (textual, color) |
|

### PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)
```


Inicializa una nueva instancia de la clase PageAreaRedaction.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Expresión regular para buscar y reemplazar |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opciones de reemplazo (textual, color) |
|
|  | imageOptions | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Opciones de reemplazo (área de imagen) |
|

### getImageOptions() {#getImageOptions--}
```
public final RegionReplacementOptions getImageOptions()
```


Obtiene el
RegionReplacementOptions
opciones con parámetros de color y área.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Aplica la redacción a una instancia de formato dada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Una instancia de un documento para aplicar la redacción |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

