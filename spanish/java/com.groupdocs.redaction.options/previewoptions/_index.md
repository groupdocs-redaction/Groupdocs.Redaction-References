---
title: "PreviewOptions"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Proporciona opciones para establecer requisitos y delegados de flujo para la generación de vistas previas."
type: docs
weight: 11
url: /es/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Proporciona opciones para establecer requisitos y delegados de flujo para la generación de vistas previas.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | Inicializa una nueva instancia de la clase PreviewOptions, provocando que el flujo de salida se cierre. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Inicializa una nueva instancia de la clase PreviewOptions, provocando que el flujo de salida se devuelva al cliente para su uso posterior. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getWidth()](#getWidth--) | Obtiene o establece el ancho de la vista previa de la página. |
|
|  | [setWidth(int value)](#setWidth-int-) | Obtiene o establece el ancho de la vista previa de la página. |
|
|  | [getHeight()](#getHeight--) | Obtiene o establece la altura de la vista previa de la página. |
|
|  | [setHeight(int value)](#setHeight-int-) | Obtiene o establece la altura de la vista previa de la página. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Obtiene o establece una matriz de números de página para generar la vista previa. |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | Obtiene o establece una matriz de números de página para generar la vista previa. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Obtiene o establece el formato de imagen de la vista previa. |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | Obtiene o establece el formato de imagen de la vista previa. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Obtiene o establece una instancia del delegado de creación de flujo de página. |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | Obtiene o establece una instancia del delegado de creación de flujo de página. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Obtiene o establece una instancia del delegado de finalización de la vista previa de la página. |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Obtiene o establece una instancia del delegado de finalización de la vista previa de la página. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Inicializa una nueva instancia de la clase PreviewOptions, provocando que el flujo de salida se cierre.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Crea un flujo para una vista previa de página específica |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Inicializa una nueva instancia de la clase PreviewOptions, provocando que el flujo de salida se devuelva al cliente para su uso posterior.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Crea un flujo para una vista previa de página específica |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Notifica que la generación de la vista previa de la página ha finalizado y obtiene el flujo de salida |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


Obtiene o establece el ancho de la vista previa de la página.


**Returns:**
int - Ancho de la vista previa de la página.

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


Obtiene o establece el ancho de la vista previa de la página.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | Ancho de la vista previa de la página. |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


Obtiene o establece la altura de la vista previa de la página.


**Returns:**
int - Altura de la vista previa de la página.

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


Obtiene o establece la altura de la vista previa de la página.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | Altura de la vista previa de la página. |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


Obtiene o establece una matriz de números de página para generar la vista previa.


**Returns:**
int[] - Una matriz de números de página para generar la vista previa.

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


Obtiene o establece una matriz de números de página para generar la vista previa.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int[] | Una matriz de números de página para generar la vista previa. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


Obtiene o establece el formato de imagen de la vista previa.


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


Obtiene o establece el formato de imagen de la vista previa.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | Formato de imagen de la vista previa. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


Obtiene o establece una instancia del delegado de creación de flujo de página.


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


Obtiene o establece una instancia del delegado de creación de flujo de página.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Una instancia del delegado de creación de flujo de página. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


Obtiene o establece una instancia del delegado de finalización de la vista previa de la página.


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


Obtiene o establece una instancia del delegado de finalización de la vista previa de la página.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Una instancia del delegado de finalización de la vista previa de la página. |
|

