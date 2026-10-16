---
title: "RasterizationOptions"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Proporciona opciones para convertir archivos a PDF."
type: docs
weight: 12
url: /es/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

Proporciona opciones para convertir archivos a PDF.

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | Inicializa una nueva instancia. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Obtiene un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un único archivo PDF. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Establece un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un único archivo PDF. |
|
|  | [getPageIndex()](#getPageIndex--) | Obtiene el índice de la primera página (basado en 0) para convertir a PDF. |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | Establece el índice de la primera página (basado en 0) para convertir a PDF. |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | Obtiene un valor que indica si la propiedad PageIndex fue modificada (establecida) después de su inicialización. |
|
|  | [getPageCount()](#getPageCount--) | Obtiene el número de páginas que se convertirán a PDF. |
|
|  | [setPageCount(int value)](#setPageCount-int-) | Establece el número de páginas que se convertirán en PDF. |
|
|  | [isPageCountSet()](#isPageCountSet--) | Obtiene un valor que indica si la propiedad PageCount fue modificada (establecida) después de su inicialización. |
|
|  | [getCompliance()](#getCompliance--) | Obtiene el nivel de cumplimiento PDF. |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | Establece el nivel de cumplimiento PDF. |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | Obtiene un indicador, que es verdadero si se establecen opciones avanzadas de rasterización. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | Puede usar este método para registrar una opción avanzada de rasterización que se aplicará. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | Puede usar este método para registrar una opción avanzada de rasterización que se aplicará. |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


Inicializa una nueva instancia.


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


Obtiene un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un único archivo PDF. TRUE por defecto, establezca FALSE para evitar la rasterización.


**Returns:**
boolean - Un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un único archivo PDF. TRUE por defecto, establezca FALSE para evitar la rasterización.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


Establece un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un único archivo PDF. TRUE por defecto, establezca FALSE para evitar la rasterización.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un único archivo PDF. TRUE por defecto, establezca FALSE para evitar la rasterización. |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Obtiene el índice de la primera página (basado en 0) para convertir a PDF.


**Returns:**
int - El índice de la primera página (basado en 0) que se convertirá en PDF.

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Establece el índice de la primera página (basado en 0) para convertir a PDF.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El índice de la primera página (basado en 0) que se convertirá en PDF. |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


Obtiene un valor que indica si la propiedad PageIndex fue modificada (establecida) después de su inicialización.


**Returns:**
boolean - Un valor que indica si la propiedad PageIndex fue modificada (establecida) después de su inicialización.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Obtiene el número de páginas que se convertirán a PDF.


**Returns:**
int - El número de páginas que se convertirán en PDF.

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Establece el número de páginas que se convertirán en PDF.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número de páginas que se convertirán en PDF. |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


Obtiene un valor que indica si la propiedad PageCount fue modificada (establecida) después de su inicialización.


**Returns:**
boolean - Un valor que indica si la propiedad PageCount fue modificada (establecida) después de su inicialización.

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


Obtiene el nivel de cumplimiento PDF.


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


Establece el nivel de cumplimiento PDF.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | El nivel de cumplimiento PDF. |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


Obtiene un indicador, que es verdadero si se establecen opciones avanzadas de rasterización.


**Returns:**
boolean - Un indicador, que es verdadero si se establecen opciones avanzadas de rasterización.

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


Puede usar este método para registrar una opción avanzada de rasterización que se aplicará.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Proporciona información sobre el tipo de efecto seleccionado (escala de grises, borde, etc.). |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


Puede usar este método para registrar una opción avanzada de rasterización que se aplicará.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Proporciona información sobre el tipo de efecto seleccionado (escala de grises, borde, etc.). |
|
|  | parámetros | java.util.HashMap<java.lang.String,java.lang.String> | Parámetros para el efecto dado, como el ángulo de rotación |
|

