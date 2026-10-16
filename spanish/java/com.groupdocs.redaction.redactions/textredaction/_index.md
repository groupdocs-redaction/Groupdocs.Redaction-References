---
title: "TextRedaction"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una clase abstracta base para redacciones de texto de documentos."
type: docs
weight: 32
url: /es/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

Representa una clase abstracta base para redacciones de texto de documentos.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Métodos

| Método | Descripción |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | Obtiene el |
ReplacementOptions
instancia, especificando el tipo de sustitución de texto.
|
|  | [getOcrConnector()](#getOcrConnector--) | Obtiene el |
IOcrConnector
implementación, requerida para extraer texto del contenido gráfico.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Establece el |
IOcrConnector
implementación, requerida para extraer texto del contenido gráfico.
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


Obtiene el
ReplacementOptions
instancia, especificando el tipo de sustitución de texto.


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Obtiene el
IOcrConnector
implementación, requerida para extraer texto del contenido gráfico.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Establece el
IOcrConnector
implementación, requerida para extraer texto del contenido gráfico.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | La implementación de IOcrConnector, requerida para extraer texto del contenido gráfico. |
|

