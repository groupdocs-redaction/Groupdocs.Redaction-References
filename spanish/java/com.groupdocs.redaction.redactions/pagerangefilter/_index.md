---
title: "PageRangeFilter"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa el filtro de redacción que establece el rango de páginas dentro de un documento para aplicar la redacción."
type: docs
weight: 24
url: /es/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

Representa un filtro de redacción, estableciendo un rango de páginas dentro de un documento para aplicar la redacción.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | Inicializa una nueva instancia de la clase RemovePageRedaction. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | Obtiene la posición de referencia de búsqueda, el comienzo o el final de un documento. |
|
|  | [getIndex()](#getIndex--) | Obtiene el índice de posición inicial (basado en 0). |
|
|  | [getCount()](#getCount--) | Obtiene la cantidad de páginas a eliminar. |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | Comprueba si este rango de páginas del filtro contiene la página dada. |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


Inicializa una nueva instancia de la clase RemovePageRedaction.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | Posición de referencia de búsqueda, el comienzo o el final de un documento |
|
|  | índice | int | Índice de posición inicial (basado en 0) |
|
|  | conteo | int | Cantidad de páginas a eliminar |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


Obtiene la posición de referencia de búsqueda, el comienzo o el final de un documento.


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Obtiene el índice de posición inicial (basado en 0).


**Returns:**
int - Índice de posición inicial (basado en cero).

### getCount() {#getCount--}
```
public final int getCount()
```


Obtiene la cantidad de páginas a eliminar.


**Returns:**
int - La cantidad de páginas a eliminar.

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


Comprueba si este rango de páginas del filtro contiene la página dada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pageIndex | int | índice de la página (basado en cero) |
|
|  | pageCount | int | recuento total de páginas |
|

**Returns:**
boolean - true, si este rango de filtro contiene página

