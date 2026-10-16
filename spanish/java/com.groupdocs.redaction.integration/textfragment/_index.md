---
title: "TextFragment"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una parte del texto reconocido, palabra, símbolo, etc., extraída por el motor OCR."
type: docs
weight: 15
url: /es/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

Representa una parte del texto reconocido (palabra, símbolo, etc.), extraído por el motor OCR.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | Inicializa una nueva instancia del fragmento de texto reconocido. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getText()](#getText--) | Obtiene el contenido textual del fragmento de texto reconocido. |
|
|  | [getRectangle()](#getRectangle--) | Obtiene un rectángulo delimitador del fragmento de texto reconocido. |
|
|  | [toString()](#toString--) | Devuelve el contenido textual del fragmento de texto reconocido. |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


Inicializa una nueva instancia del fragmento de texto reconocido.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | texto | java.lang.String | contenido textual del fragmento de texto reconocido |
|
|  | rectángulo | java.awt.Rectangle | rectángulo delimitador del fragmento de texto reconocido |
|

### getText() {#getText--}
```
public final String getText()
```


Obtiene el contenido textual del fragmento de texto reconocido.


**Returns:**
java.lang.String - Un contenido textual del fragmento de texto reconocido.

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Obtiene un rectángulo delimitador del fragmento de texto reconocido.


**Returns:**
java.awt.Rectangle - Un rectángulo delimitador del fragmento de texto reconocido.

### toString() {#toString--}
```
public String toString()
```


Devuelve el contenido textual del fragmento de texto reconocido.


**Returns:**
java.lang.String - contenido textual del fragmento de texto reconocido

