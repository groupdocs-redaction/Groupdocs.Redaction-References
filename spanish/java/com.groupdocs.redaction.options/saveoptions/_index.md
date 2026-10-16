---
title: "SaveOptions"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Proporciona opciones para cambiar el nombre del archivo de salida y/o convertir el documento a rasterización PDF basada en imágenes."
type: docs
weight: 14
url: /es/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

Proporciona opciones para cambiar el nombre del archivo de salida y/o convertir el documento a PDF basado en imágenes (rasterización).

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | Inicializa una nueva instancia con valores predeterminados: rasterizar a PDF - false, agregar sufijo - false. |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | Inicializa una nueva instancia con los parámetros dados. |
|
## Campos

| Campo | Descripción |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | Representa el valor predeterminado del sufijo, que es "Redacted". |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | Obtiene un valor que indica si el nombre del archivo necesita ser cambiado antes de guardar. |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | Establece un valor que indica si el nombre del archivo necesita ser cambiado antes de guardar. |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | Obtiene un sufijo personalizado para el nombre del archivo de salida. |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | Establece un sufijo personalizado para el nombre del archivo de salida. |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | Obtiene un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un único archivo PDF. |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | Establece un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un único archivo PDF. |
|
|  | [getRasterization()](#getRasterization--) | Obtiene la configuración de rasterización. |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | Opciones de guardado de procesamiento de texto. |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


Inicializa una nueva instancia con valores predeterminados: rasterizar a PDF - false, agregar sufijo - false.


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


Inicializa una nueva instancia con los parámetros dados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | True, si todas las páginas del documento deben convertirse en imágenes y colocarse en un único archivo PDF |
|
|  | suffix | java.lang.String | Este texto se añadirá al final del nombre del archivo; si no está vacío, también establece AddSuffix en true |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


Representa el valor predeterminado del sufijo, que es "Redacted".


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


Obtiene un valor que indica si el nombre del archivo necesita ser cambiado antes de guardar. False por defecto.


**Returns:**
boolean - Un valor que indica si el nombre del archivo necesita ser cambiado antes de guardar. False por defecto.

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


Establece un valor que indica si el nombre del archivo necesita ser cambiado antes de guardar. False por defecto.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si el nombre del archivo necesita ser cambiado antes de guardar. False por defecto. |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


Obtiene un sufijo personalizado para el nombre del archivo de salida. Si no se especifica, el
SaveSuffix
constante será utilizada.


**Returns:**
java.lang.String - Un sufijo personalizado para el nombre del archivo de salida. Si no se especifica, la constante  SaveSuffix  será utilizada.

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


Establece un sufijo personalizado para el nombre del archivo de salida. Si no se especifica, el
SaveSuffix
constante será utilizada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | Un sufijo personalizado para el nombre del archivo de salida. Si no se especifica, se utilizará la constante  SaveSuffix  . |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


Obtiene un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un único archivo PDF.


**Returns:**
boolean - Un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un solo archivo PDF.

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


Establece un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un único archivo PDF.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un solo archivo PDF. |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


Obtiene la configuración de rasterización.


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


Opciones de guardado de procesamiento de texto.


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
