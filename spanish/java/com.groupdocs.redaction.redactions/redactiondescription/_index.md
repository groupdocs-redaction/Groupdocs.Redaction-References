---
title: "RedactionDescription"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa la información de una única acción de cambio que se realiza durante el proceso de redacción."
type: docs
weight: 25
url: /es/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

Representa la información de una única acción de cambio que se realiza durante el proceso de redacción.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | Inicializa una nueva instancia de la clase RedactionDescription sin información de reemplazo. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | Inicializa una nueva instancia de la clase RedactionDescription con información de reemplazo. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | Inicializa una nueva instancia de la clase RedactionDescription con información de reemplazo de área de imagen. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | Obtiene el tipo de datos del documento: texto, metadatos o anotaciones. |
|
|  | [getActionType()](#getActionType--) | Obtiene la operación de redacción: reemplazo, limpieza o eliminación. |
|
|  | [getOriginalText()](#getOriginalText--) | Obtiene el texto coincidente, si se proporciona alguna expresión. |
|
|  | [getReplacement()](#getReplacement--) | Obtiene la información de reemplazo, puede ser nula. |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | Obtiene la información de reemplazo para redacciones de áreas de imagen, devuelve nulo para redacciones textuales. |
|
|  | [getDetails()](#getDetails--) | Obtiene una información de detalles opcional para el elemento que se está redactando. |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | Establece una información de detalles opcional para el elemento que se está redactando. |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


Inicializa una nueva instancia de la clase RedactionDescription sin información de reemplazo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | redactionType | int | Tipo de datos que se están redactando |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Acción a realizar sobre estos datos |
|
|  | originalText | java.lang.String | Texto coincidente, comentario o cuerpo de anotación |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


Inicializa una nueva instancia de la clase RedactionDescription con información de reemplazo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | redactionType | int | Tipo de datos que se están redactando |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Acción a realizar sobre estos datos |
|
|  | originalText | java.lang.String | Texto coincidente, comentario o cuerpo de anotación |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | Texto de reemplazo, texto coincidente y su posición dentro de la cadena original |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


Inicializa una nueva instancia de la clase RedactionDescription con información de reemplazo de área de imagen.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | redactionType | int | Tipo de datos que se están redactando |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Acción a realizar sobre estos datos |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Información de reemplazo del área de imagen |
|
|  | imageDetails | java.lang.String | Descripción textual de la imagen, por defecto es String.Empty |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


Obtiene el tipo de datos del documento: texto, metadatos o anotaciones.


**Returns:**
int - El tipo de datos del documento - texto, metadatos o anotaciones.

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


Obtiene la operación de redacción: reemplazo, limpieza o eliminación.


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Obtiene el texto coincidente, si se proporciona alguna expresión.


**Returns:**
java.lang.String - El texto coincidente, si se proporciona alguna expresión.

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


Obtiene la información de reemplazo, puede ser nula.


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


Obtiene la información de reemplazo para redacciones de áreas de imagen, devuelve nulo para redacciones textuales.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


Obtiene una información de detalles opcional para el elemento que se está redactando.


**Returns:**
java.lang.String - Una información de detalles opcional para el elemento que se está redactando.

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


Establece una información de detalles opcional para el elemento que se está redactando.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | Una información de detalles opcional para el elemento que se está redactando. |
|

