---
title: "ImageAreaRedaction"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una redacción que coloca un rectángulo de color en el área dada de un documento de imagen."
type: docs
weight: 18
url: /es/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

Representa una redacción que coloca un rectángulo de color en el área dada de un documento de imagen.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Inicializa una nueva instancia de la clase ImageAreaRedaction para redactar un tamaño de área específico. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getOptions()](#getOptions--) | Obtiene el |
RegionReplacementOptions
opciones con parámetros de color y área.
|
|  | [getTopLeft()](#getTopLeft--) | Obtiene la posición superior izquierda del área a eliminar |
|
|  | [getDescription()](#getDescription--) | Devuelve una cadena que describe la redacción y sus parámetros. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Aplica la redacción a una instancia de formato dada. |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


Inicializa una nueva instancia de la clase ImageAreaRedaction para redactar un tamaño de área específico.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Coordenadas del área superior izquierda |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Tamaño y color del área |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


Obtiene el
RegionReplacementOptions
opciones con parámetros de color y área.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


Obtiene la posición superior izquierda del área a eliminar


**Returns:**
java.awt.Point - La posición superior izquierda del área a eliminar

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

