---
title: "RecognizedImage"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa el texto extraído de una imagen como resultado de su proceso de reconocimiento."
type: docs
weight: 13
url: /es/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

Representa texto, extraído de una imagen como resultado de su proceso de reconocimiento.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | Inicializa una nueva instancia de la clase, usando un conjunto de líneas reconocidas. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getText()](#getText--) | Obtiene el equivalente textual del texto estructurado. |
|
|  | [getLines()](#getLines--) | Obtiene las líneas de texto, con sus fragmentos, reconocidas dentro del documento. |
|
|  | [toString()](#toString--) | Obtiene el equivalente textual del texto estructurado. |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


Inicializa una nueva instancia de la clase, usando un conjunto de líneas reconocidas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | un IEnumerable (p.ej., una lista o una matriz) de líneas reconocidas |
|

### getText() {#getText--}
```
public final String getText()
```


Obtiene el equivalente textual del texto estructurado.


**Returns:**
java.lang.String - Equivalente textual del texto estructurado.

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


Obtiene las líneas de texto, con sus fragmentos, reconocidas dentro del documento.


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - Líneas de texto, con sus fragmentos, reconocidas dentro del documento.

### toString() {#toString--}
```
public String toString()
```


Obtiene el equivalente textual del texto estructurado.


**Returns:**
java.lang.String - Texto reconocido

