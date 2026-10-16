---
title: "RegexRedaction"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una redacción de texto que busca y reemplaza texto en el documento coincidiendo con la expresión regular proporcionada."
type: docs
weight: 28
url: /es/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

Representa una redacción de texto que busca y reemplaza texto en el documento coincidiendo con la expresión regular proporcionada.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Inicializa una nueva instancia de la clase RegexRedaction. |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Inicializa una nueva instancia de la clase RegexRedaction. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | Obtiene la expresión regular a coincidir. |
|
|  | [getDescription()](#getDescription--) | Devuelve una cadena que describe la redacción y sus parámetros. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Aplica la redacción a una instancia de formato dada. |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


Inicializa una nueva instancia de la clase RegexRedaction.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | patrón | java.lang.String | Expresión regular para buscar y reemplazar |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opciones de reemplazo (textual, color) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


Inicializa una nueva instancia de la clase RegexRedaction.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Expresión regular para buscar y reemplazar |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opciones de reemplazo (textual, color) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


Obtiene la expresión regular a coincidir.


**Returns:**
java.util.regex.Pattern - La expresión regular a coincidir.

### getDescription() {#getDescription--}
```
public String getDescription()
```


Devuelve una cadena que describe la redacción y sus parámetros.


**Returns:**
java.lang.String - Texto que contiene el nombre de la redacción y los parámetros.

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

