---
title: "TextReplacement"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa información de reemplazo textual."
type: docs
weight: 33
url: /es/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

Representa información de reemplazo textual.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | Inicializa una nueva instancia de la clase TextReplacement. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getIndex()](#getIndex--) | Obtiene un índice del texto coincidente dentro de la cadena fuente. |
|
|  | [getOriginalText()](#getOriginalText--) | Obtiene la cadena original coincidente. |
|
|  | [getReplacement()](#getReplacement--) | Obtiene la cadena, reemplazando OriginalText. |
|
|  | [toString()](#toString--) | Proporciona la descripción del reemplazo de texto y su posición. |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


Inicializa una nueva instancia de la clase TextReplacement.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índice | int | Índice de un texto coincidente dentro de la cadena fuente |
|
|  | original | java.lang.String | Cadena original coincidente |
|
|  | reemplazo | java.lang.String | Cadena, reemplazando OriginalText en la cadena fuente |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Obtiene un índice del texto coincidente dentro de la cadena fuente.


**Returns:**
int - Un índice del texto coincidente dentro de la cadena fuente.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Obtiene la cadena original coincidente.


**Returns:**
java.lang.String - La cadena original coincidente.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Obtiene la cadena, reemplazando OriginalText.


**Returns:**
java.lang.String - La cadena, reemplazando OriginalText.

### toString() {#toString--}
```
public String toString()
```


Proporciona la descripción del reemplazo de texto y su posición.


**Returns:**
java.lang.String - Descripción del reemplazo

