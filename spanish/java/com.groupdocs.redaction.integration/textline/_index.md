---
title: "TextLine"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una línea de texto extraída por el motor OCR de una imagen."
type: docs
weight: 16
url: /es/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

Representa una línea de texto, extraída por el motor OCR de una imagen.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | Inicializa una nueva instancia de una línea de texto, extraída por el motor OCR de una imagen. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFragments()](#getFragments--) | Obtiene una matriz de fragmentos de texto, como símbolos y palabras, reconocidos en la línea. |
|
|  | [toString()](#toString--) | Devuelve el contenido textual de la línea de texto reconocida. |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


Inicializa una nueva instancia de una línea de texto, extraída por el motor OCR de una imagen.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | conjunto inicial de fragmentos de texto |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


Obtiene una matriz de fragmentos de texto, como símbolos y palabras, reconocidos en la línea.


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - Una matriz de fragmentos de texto, como símbolos y palabras, reconocidos en la línea.

### toString() {#toString--}
```
public String toString()
```


Devuelve el contenido textual de la línea de texto reconocida.


**Returns:**
java.lang.String - contenido textual de la línea de texto reconocida

