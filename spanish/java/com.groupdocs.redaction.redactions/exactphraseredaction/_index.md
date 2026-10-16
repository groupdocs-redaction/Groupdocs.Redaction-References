---
title: "ExactPhraseRedaction"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una redacción de texto que reemplaza una frase exacta en el texto del documento sin distinción de mayúsculas por defecto."
type: docs
weight: 17
url: /es/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

Representa una redacción de texto que reemplaza una frase exacta en el texto del documento, sin distinción de mayúsculas por defecto.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

El siguiente ejemplo demuestra la realización de una búsqueda y reemplazo de frases sensible a mayúsculas.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
``` 
````

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

````

try (Redactor redactor = new Redactor("C:\\sample.pdf"))
{
// Por defecto, isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
doc.save();
}
 
``` 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Inicializa una nueva instancia de la clase ExactPhraseRedaction en modo sin distinción de mayúsculas. |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | Inicializa una nueva instancia de la clase ExactPhraseRedaction. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | Obtiene la cadena a buscar y reemplazar. |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | Obtiene un valor que indica si la búsqueda distingue mayúsculas y minúsculas o no. |
|
|  | [isRightToLeft()](#isRightToLeft--) | Obtiene un valor que indica si este texto es de derecha a izquierda o no, false por defecto. |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | Establece un valor que indica si este texto es de derecha a izquierda o no, false por defecto. |
|
|  | [getDescription()](#getDescription--) | Devuelve una cadena que describe la redacción y sus parámetros. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Aplica la redacción a una instancia de formato dada. |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


Inicializa una nueva instancia de la clase ExactPhraseRedaction en modo sin distinción de mayúsculas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Cadena a buscar y reemplazar |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opciones de reemplazo (textual, color) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


Inicializa una nueva instancia de la clase ExactPhraseRedaction.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Cadena a buscar y reemplazar |
|
|  | isCaseSensitive | boolean | True si se requiere una búsqueda que distinga mayúsculas y minúsculas |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opciones de reemplazo (textual, color) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


Obtiene la cadena a buscar y reemplazar.


**Returns:**
java.lang.String - La cadena a buscar y reemplazar.

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


Obtiene un valor que indica si la búsqueda distingue mayúsculas y minúsculas o no.


**Returns:**
boolean - Un valor que indica si la búsqueda distingue mayúsculas y minúsculas o no.

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


Obtiene un valor que indica si este texto es de derecha a izquierda o no, false por defecto.


**Returns:**
boolean - Un valor que indica si este texto es de derecha a izquierda o no, false por defecto.

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


Establece un valor que indica si este texto es de derecha a izquierda o no, false por defecto.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si este texto es de derecha a izquierda o no, false por defecto. |
|

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

