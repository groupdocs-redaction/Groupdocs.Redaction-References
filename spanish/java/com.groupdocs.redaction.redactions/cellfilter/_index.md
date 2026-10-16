---
title: "CellFilter"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Proporciona una opción para limitar el alcance de una CellColumnRedaction a una hoja de cálculo y una columna."
type: docs
weight: 12
url: /es/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

Proporciona una opción para limitar el alcance de un
CellColumnRedaction
a una hoja de cálculo y una columna.

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | Inicializa una nueva instancia. |
|
## Campos

| Campo | Descripción |
| --- | --- |
|  | [NoIndex](#NoIndex) | Representa un valor predeterminado para el filtro, que es -1. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | Obtiene el nombre de la hoja de cálculo (si corresponde). |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | Establece el nombre de la hoja de cálculo (si corresponde). |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | Obtiene el índice de la hoja de cálculo (basado en cero). |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | Establece el índice de la hoja de cálculo (basado en cero). |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | Obtiene un valor que indica si el |
WorkSheetIndex
está configurado o no.
|
|  | [getColumnIndex()](#getColumnIndex--) | Obtiene un índice de columna (basado en cero). |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | Establece un índice de columna (basado en cero). |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


Inicializa una nueva instancia.


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


Representa un valor predeterminado para el filtro, que es -1.


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


Obtiene el nombre de la hoja de cálculo (si corresponde).


**Returns:**
java.lang.String - Un nombre de hoja de cálculo (si corresponde).

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


Establece el nombre de la hoja de cálculo (si corresponde).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | Un nombre de hoja de cálculo (si corresponde). |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


Obtiene el índice de la hoja de cálculo (basado en cero).


**Returns:**
int - Un índice de hoja de cálculo (basado en cero).

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


Establece el índice de la hoja de cálculo (basado en cero).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | Un índice de hoja de cálculo (basado en cero). |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


Obtiene un valor que indica si el
WorkSheetIndex
está configurado o no.


**Returns:**
boolean - Un valor que indica si el  WorkSheetIndex  está configurado o no.

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


Obtiene un índice de columna (basado en cero).


**Returns:**
int - Un índice de columna (basado en cero).

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


Establece un índice de columna (basado en cero).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | Un índice de columna (basado en cero). |
|

