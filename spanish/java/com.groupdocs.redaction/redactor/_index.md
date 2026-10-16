---
title: "Redactor"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una clase principal que controla el proceso de redacción de documentos, permitiendo abrir, redactar y guardar documentos."
type: docs
weight: 16
url: /es/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

Representa una clase principal que controla el proceso de redacción de documentos, permitiendo abrir, redactar y guardar documentos.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | Inicializa una nueva instancia de |
Redactor
clase usando la ruta del archivo.
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | Inicializa una nueva instancia de |
Redactor
clase usando un flujo.
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | Inicializa una nueva instancia de |
Redactor
clase para un documento protegido con contraseña usando su ruta.
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Inicializa una nueva instancia de |
Redactor
clase para un documento protegido con contraseña usando su ruta y configuraciones.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | Inicializa una nueva instancia de |
Redactor
clase para un documento protegido con contraseña usando un flujo.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Inicializa una nueva instancia de |
Redactor
clase para un documento protegido con contraseña usando un flujo y configuraciones.
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [close()](#close--) | Libera recursos. |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | Aplica una redacción al documento. |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | Aplica un conjunto de redacciones al documento. |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | Aplica una política de redacción al documento. |
|
|  | [save()](#save--) | Guarda el documento en un archivo con las siguientes opciones: AddSuffix = true, RasterizeToPDF = true. |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | Guarda el documento en un archivo. |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | Guarda el documento en un flujo. |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | Guarda el documento en un flujo. |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | Guarda el documento en un flujo, incluyendo ubicación personalizada. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | Genera imágenes de vista previa de páginas específicas en un formato de imagen dado. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Obtiene la información general del documento: tamaño, número de páginas, etc. |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


Inicializa una nueva instancia de
Redactor
clase usando la ruta del archivo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | Ruta al archivo |


El siguiente ejemplo muestra cómo abrir un documento para redacción.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
     // Here we can use document instance to perform redactions
 }
 
``` 
````

 |

### Redactor(InputStream document) {#Redactor-java.io.InputStream-}
```
public Redactor(InputStream document)
```


Initializes a new instance of 
Redactor
 class using stream.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source stream of the document


The following example demonstrates how to open a document from stream.

````

try (InputStream stream = new FileInputStream("C:\\sample.pdf"))
{
try (Redactor redactor = new Redactor(stream))
{
// Aquí podemos usar la instancia del documento para realizar redacciones
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


Inicializa una nueva instancia de
Redactor
clase para un documento protegido con contraseña usando su ruta.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | Ruta al archivo. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opciones, incluida la contraseña. |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


Inicializa una nueva instancia de
Redactor
clase para un documento protegido con contraseña usando su ruta y configuraciones.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | Ruta al archivo. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opciones dependientes del archivo, incluida la contraseña. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Configuración predeterminada para el proceso de redacción. |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


Inicializa una nueva instancia de
Redactor
clase para un documento protegido con contraseña usando un flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documento | java.io.InputStream | Flujo de entrada de origen. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opciones, incluida la contraseña. |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


Inicializa una nueva instancia de
Redactor
clase para un documento protegido con contraseña usando un flujo y configuraciones.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documento | java.io.InputStream | Flujo de entrada de origen. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opciones, incluida la contraseña. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Configuración predeterminada para el proceso de redacción. |
|

### close() {#close--}
```
public final void close()
```


Libera recursos.


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


Aplica una redacción al documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Una instancia de  Redaction  para aplicar |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


Aplica un conjunto de redacciones al documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Una matriz de redacciones para aplicar |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


Aplica una política de redacción al documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | Política de redacción |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


Guarda el documento en un archivo con las siguientes opciones: AddSuffix = true, RasterizeToPDF = true.


**Returns:**
java.lang.String - Ruta al documento redactado

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


Guarda el documento en un archivo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Opciones para agregar sufijo o rasterizar |
|

**Returns:**
java.lang.String - Ruta al documento redactado

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


Guarda el documento en un flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documento | java.io.OutputStream | Flujo de destino |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


Guarda el documento en un flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documento | java.io.OutputStream | Flujo de destino |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Opciones de guardado |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


Guarda el documento en un flujo, incluyendo ubicación personalizada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documento | java.io.OutputStream | Flujo de destino |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | Opciones para rasterizar o no y para especificar páginas para la rasterización |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


Genera imágenes de vista previa de páginas específicas en un formato de imagen dado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | Propiedades de imagen y configuraciones de rango de páginas |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


Obtiene la información general del documento: tamaño, número de páginas, etc.


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

