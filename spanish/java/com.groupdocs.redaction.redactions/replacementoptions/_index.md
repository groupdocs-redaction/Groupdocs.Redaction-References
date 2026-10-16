---
title: "ReplacementOptions"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa opciones para el reemplazo de texto coincidente."
type: docs
weight: 31
url: /es/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

Representa opciones para el reemplazo de texto coincidente.

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | Inicializa una nueva instancia de la clase ReplacementOptions con texto de reemplazo como opción. |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | Inicializa una nueva instancia de la clase ReplacementOptions con rectángulo coloreado como opción. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getActionType()](#getActionType--) | Obtiene la acción de reemplazo: dibujar cuadro o reemplazar texto. |
|
|  | [getReplacement()](#getReplacement--) | Obtiene el valor de reemplazo textual. |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | Establece el valor de reemplazo textual. |
|
|  | [getBoxColor()](#getBoxColor--) | Obtiene el color para un |
ReplacementType.DrawBox
opción (ignorada de otro modo).
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | Establece el color para un |
ReplacementType.DrawBox
opción (ignorada de otro modo).
|
|  | [getFilters()](#getFilters--) | Obtiene una matriz de filtros para aplicar con esta redacción. |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | Establece una matriz de filtros para aplicar con esta redacción. |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | Obtiene un controlador de redacción personalizado. |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | Establece un controlador de redacción personalizado. |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


Inicializa una nueva instancia de la clase ReplacementOptions con texto de reemplazo como opción.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | reemplazo | java.lang.String | Reemplazo textual |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


Inicializa una nueva instancia de la clase ReplacementOptions con rectángulo coloreado como opción.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | color | java.awt.Color | Color del rectángulo |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


Obtiene la acción de reemplazo: dibujar cuadro o reemplazar texto.


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Obtiene el valor de reemplazo textual.


**Returns:**
java.lang.String - El valor de reemplazo textual.

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


Establece el valor de reemplazo textual.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | El valor de reemplazo textual. |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


Obtiene el color para un
ReplacementType.DrawBox
opción (ignorada de otro modo).


**Returns:**
java.awt.Color - El color para una  ReplacementType.DrawBox  opción (ignorada de otro modo).

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


Establece el color para un
ReplacementType.DrawBox
opción (ignorada de otro modo).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.awt.Color | El color para una  ReplacementType.DrawBox  opción (ignorada de otro modo). |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


Obtiene una matriz de filtros para aplicar con esta redacción.


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - Una matriz de filtros para aplicar con esta redacción.

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


Establece una matriz de filtros para aplicar con esta redacción.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | Una matriz de filtros para aplicar con esta redacción. |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


Obtiene un controlador de redacción personalizado. Compatible solo con PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


Establece un controlador de redacción personalizado. Compatible solo con PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | Una instancia de [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler). |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
