---
title: "PageAreaFilter"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa un filtro de redacción que establece un área dentro de una página de un documento para aplicar la redacción."
type: docs
weight: 22
url: /es/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

Representa un filtro de redacción, estableciendo un área dentro de una página de un documento para aplicar la redacción.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | Inicializa una nueva instancia de la clase PageAreaFilter para redactar un área específica. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtiene el rectángulo (posición superior izquierda y tamaño del área) en una página. |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | Comprueba si esta área del filtro tiene intersección con el rectángulo dado. |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


Inicializa una nueva instancia de la clase PageAreaFilter para redactar un área específica.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Coordenadas del área superior izquierda |
|
|  | tamaño | java.awt.Dimension | Tamaño y color del área |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Obtiene el rectángulo (posición superior izquierda y tamaño del área) en una página.


**Returns:**
java.awt.Rectangle - El rectángulo (posición superior izquierda y tamaño del área) en una página.

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


Comprueba si esta área del filtro tiene intersección con el rectángulo dado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectángulo | java.awt.Rectangle | Rectángulo a comprobar |
|

**Returns:**
boolean - true, si esta área del filtro tiene intersección

