---
title: "RedactableImage"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Proporciona una fachada para todas las operaciones de redacción de imágenes raster."
type: docs
weight: 14
url: /es/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

Proporciona una fachada para todas las operaciones de redacción de imágenes raster.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | Crea una nueva instancia usando un objeto, que implementa |
IImageFormatInstance
interfaz.
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | Crea una nueva instancia usando un objeto, que implementa |
IMultipleAreaRedactable
interfaz.
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | Recupera un flujo con el contenido real de la imagen. |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Redacta múltiples áreas de imagen a la vez con el mismo color. |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Reemplaza el área en el punto dado con un rectángulo de color y tamaño específicos. |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


Crea una nueva instancia usando un objeto, que implementa
IImageFormatInstance
interfaz.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | Una instancia, que implementa la interfaz IImageFormatInstance |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


Crea una nueva instancia usando un objeto, que implementa
IMultipleAreaRedactable
interfaz.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | Una instancia, que implementa la interfaz IMultipleAreaRedactable |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


Recupera un flujo con el contenido real de la imagen.


**Returns:**
java.io.InputStream - Flujo, que contiene datos de imagen

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


Redacta múltiples áreas de imagen a la vez con el mismo color.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectángulos | java.awt.Rectangle[] | Una matriz de áreas rectangulares |
|
|  | boxColor | java.awt.Color | Color para rellenar las áreas |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Reemplaza el área en el punto dado con un rectángulo de color y tamaño específicos.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Coordenadas de la esquina superior izquierda del área rellenada |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Configuración de color y tamaño |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

