---
title: "MetadataFilters"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una lista de los tipos de metadatos de documento más comunes."
type: docs
weight: 19
url: /es/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

Representa una lista de los tipos de metadatos de documento más comunes.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## Campos

| Campo | Descripción |
| --- | --- |
|  | [None](#None) | Configuración de filtro vacío, no coincide con ningún elemento de metadatos. |
|
|  | [Author](#Author) | Autor del documento. |
|
|  | [Category](#Category) | Categoría del documento. |
|
|  | [Comments](#Comments) | Comentario del documento. |
|
|  | [Company](#Company) | Empresa del Autor. |
|
|  | [ContentStatus](#ContentStatus) | Estado del contenido. |
|
|  | [CreatedTime](#CreatedTime) | Hora de creación. |
|
|  | [HyperlinkBase](#HyperlinkBase) | Base del hipervínculo. |
|
|  | [LastPrinted](#LastPrinted) | Fecha y hora de la última impresión. |
|
|  | [LastSavedBy](#LastSavedBy) | Última guardada por el usuario. |
|
|  | [LastSavedTime](#LastSavedTime) | Fecha y hora de la última guardada. |
|
|  | [NameOfApplication](#NameOfApplication) | Nombre de la aplicación donde se creó el documento. |
|
|  | [Manager](#Manager) | Nombre del gerente del autor. |
|
|  | [RevisionNumber](#RevisionNumber) | Número de revisión. |
|
|  | [Subject](#Subject) | Asunto del documento. |
|
|  | [Template](#Template) | Nombre de la plantilla del documento. |
|
|  | [Title](#Title) | Título del documento. |
|
|  | [TotalEditingTime](#TotalEditingTime) | Tiempo total de edición. |
|
|  | [Version](#Version) | Versión del documento. |
|
|  | [Description](#Description) | Descripción del documento. |
|
|  | [Keywords](#Keywords) | Palabras clave del documento. |
|
|  | [ContentType](#ContentType) | Tipo de contenido. |
|
|  | [All](#All) | Todos los tipos de los elementos de metadatos. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getNames()](#getNames--) | Obtiene un conjunto con todos los tipos de filtro declarados. |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | Obtiene el valor de MetadataFiler por su nombre. |
|
|  | [parse(String values)](#parse-java.lang.String-) | Analiza una cadena de valores de MetadataFilers delimitados por comas a un entero. |
|
|  | [toString(int value)](#toString-int-) | Guarda un entero como una cadena de valores de MetadataFilers delimitados por comas. |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


Configuración de filtro vacío, no coincide con ningún elemento de metadatos.


### Author {#Author}
```
public static final int Author
```


Autor del documento.


### Category {#Category}
```
public static final int Category
```


Categoría del documento.


### Comments {#Comments}
```
public static final int Comments
```


Comentario del documento.


### Company {#Company}
```
public static final int Company
```


Empresa del Autor.


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


Estado del contenido.


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


Hora de creación.


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


Base del hipervínculo.


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


Fecha y hora de la última impresión.


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


Última guardada por el usuario.


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


Fecha y hora de la última guardada.


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


Nombre de la aplicación donde se creó el documento.


### Manager {#Manager}
```
public static final int Manager
```


Nombre del gerente del autor.


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


Número de revisión.


### Subject {#Subject}
```
public static final int Subject
```


Asunto del documento.


### Template {#Template}
```
public static final int Template
```


Nombre de la plantilla del documento.


### Title {#Title}
```
public static final int Title
```


Título del documento.


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


Tiempo total de edición.


### Version {#Version}
```
public static final int Version
```


Versión del documento.


### Description {#Description}
```
public static final int Description
```


Descripción del documento.


### Keywords {#Keywords}
```
public static final int Keywords
```


Palabras clave del documento.


### ContentType {#ContentType}
```
public static final int ContentType
```


Tipo de contenido.


### All {#All}
```
public static final int All
```


Todos los tipos de los elementos de metadatos.


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


Obtiene un conjunto con todos los tipos de filtro declarados.


**Returns:**
java.util.Set<java.lang.String> - Un conjunto con todos los tipos de filtro declarados.

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


Obtiene el valor de MetadataFiler por su nombre.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valueName | java.lang.String | Nombre de MetadataFilter. |
|

**Returns:**
int - Valor de MetadataFiler.

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


Analiza una cadena de valores de MetadataFilers delimitados por comas a un entero.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valores | java.lang.String | Una cadena de valores de MetadataFilers delimitados por comas. |
|

**Returns:**
int - Valor de MetadataFilers.

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


Guarda un entero como una cadena de valores de MetadataFilers delimitados por comas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | Valor de MetadataFiler. |
|

**Returns:**
java.lang.String - Una cadena de valores de MetadataFiler delimitados por comas.

