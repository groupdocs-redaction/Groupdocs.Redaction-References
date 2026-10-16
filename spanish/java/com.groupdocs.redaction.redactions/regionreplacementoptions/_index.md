---
title: "RegionReplacementOptions"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa los parámetros de color y área para el reemplazo de regiones de imagen."
type: docs
weight: 29
url: /es/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

Representa parámetros de color y área para la sustitución de regiones de imagen. Ver
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | Inicializa una nueva instancia de la clase RegionReplacementOptions. |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | Inicializa una nueva instancia de la clase RegionReplacementOptions cuyo tamaño coincide con el texto dado. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | Obtiene el color para rellenar el área redactada. |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | Establece el color para rellenar el área redactada. |
|
|  | [getSize()](#getSize--) | Obtiene el rectángulo con ancho y altura. |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | Establece el rectángulo con ancho y altura. |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


Inicializa una nueva instancia de la clase RegionReplacementOptions.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Color para rellenar el área |
|
|  | tamaño | java.awt.Dimension | Tamaño del área rellenada |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


Inicializa una nueva instancia de la clase RegionReplacementOptions cuyo tamaño coincide con el texto dado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Color para rellenar el área |
|
|  | font | java.awt.Font | Fuente del texto esperado |
|
|  | expectedText | java.lang.String | Texto esperado |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


Obtiene el color para rellenar el área redactada.


**Returns:**
java.awt.Color - El color para rellenar el área redactada.

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


Establece el color para rellenar el área redactada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.awt.Color | El color para rellenar el área redactada. |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


Obtiene el rectángulo con ancho y altura.


**Returns:**
java.awt.Dimension - El rectángulo con ancho y altura.

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


Establece el rectángulo con ancho y altura.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.awt.Dimension | El rectángulo con ancho y altura. |
|

