---
title: "MetadataItem"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa un elemento de metadatos común a todos los formatos compatibles y utilizado en redactado de metadatos."
type: docs
weight: 12
url: /es/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Representa un elemento de metadatos, común para todos los formatos compatibles y usado en redactado de metadatos.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | Inicializa una nueva instancia. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | Obtiene el nombre original del elemento de metadatos, tal como aparece en el documento. |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | Establece el nombre original del elemento de metadatos, tal como aparece en el documento. |
|
|  | [getCategory()](#getCategory--) | Obtiene una categoría del elemento de metadatos, por ejemplo el ID de recurso para un elemento de metadatos de recurso incrustado. |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | Establece una categoría del elemento de metadatos, por ejemplo el ID de recurso para un elemento de metadatos de recurso incrustado. |
|
|  | [getFilter()](#getFilter--) | Obtiene un valor de |
MetadataFilters
, asignado a este elemento de metadatos que se utiliza en la filtración de elementos.
|
|  | [setFilter(int value)](#setFilter-int-) | Establece un valor de |
MetadataFilters
, asignado a este elemento de metadatos que se utiliza en la filtración de elementos.
|
|  | [getValues()](#getValues--) | Obtiene el valor del elemento de metadatos. |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | Establece el valor del elemento de metadatos. |
|
|  | [isCustom()](#isCustom--) | Obtiene un valor que indica si este elemento es personalizado (agregado por los autores del documento). |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | Establece un valor que indica si este elemento es personalizado (agregado por los autores del documento). |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | Obtiene una clave de diccionario para , usando su OriginalName y otros datos. |
|
|  | [createClone()](#createClone--) | Crea una clonación profunda de la instancia actual. |
|
|  | [getActualValue()](#getActualValue--) | Obtiene la representación en cadena del valor del elemento de metadatos. |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


Inicializa una nueva instancia.


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


Obtiene el nombre original del elemento de metadatos, tal como aparece en el documento.


**Returns:**
java.lang.String - Un nombre original del elemento de metadatos, tal como aparece en el documento.

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


Establece el nombre original del elemento de metadatos, tal como aparece en el documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | Un nombre original del elemento de metadatos, tal como aparece en el documento. |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


Obtiene una categoría del elemento de metadatos, por ejemplo el ID de recurso para un elemento de metadatos de recurso incrustado.


**Returns:**
java.lang.String - Una categoría del elemento de metadatos, por ejemplo el ID de recurso para un elemento de metadatos de recurso incrustado.

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Establece una categoría del elemento de metadatos, por ejemplo el ID de recurso para un elemento de metadatos de recurso incrustado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | Una categoría del elemento de metadatos, por ejemplo el ID de recurso para un elemento de metadatos de recurso incrustado. |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


Obtiene un valor de
MetadataFilters
, asignado a este elemento de metadatos que se utiliza en la filtración de elementos.


**Returns:**
int - Un valor de  MetadataFilters , asignado a este elemento de metadatos que se utiliza en la filtración de elementos.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Establece un valor de
MetadataFilters
, asignado a este elemento de metadatos que se utiliza en la filtración de elementos.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | Un valor de  MetadataFilters , asignado a este elemento de metadatos que se utiliza en la filtración de elementos. |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


Obtiene el valor del elemento de metadatos.


**Returns:**
java.util.List<java.lang.String> - El valor del elemento de metadatos.

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


Establece el valor del elemento de metadatos.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.util.List<java.lang.String> | El valor del elemento de metadatos. |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


Obtiene un valor que indica si este elemento es personalizado (agregado por los autores del documento).


**Returns:**
boolean - Un valor que indica si este elemento es personalizado (agregado por los autores del documento).

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


Establece un valor que indica si este elemento es personalizado (agregado por los autores del documento).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si este elemento es personalizado (agregado por los autores del documento). |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


Obtiene una clave de diccionario para , usando su OriginalName y otros datos.


**Returns:**
java.lang.String - Una clave de diccionario para , usando su OriginalName y otros datos.

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


Crea una clonación profunda de la instancia actual.


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


Obtiene la representación en cadena del valor del elemento de metadatos.


**Returns:**
java.lang.String - La representación en cadena del valor del elemento de metadatos.

