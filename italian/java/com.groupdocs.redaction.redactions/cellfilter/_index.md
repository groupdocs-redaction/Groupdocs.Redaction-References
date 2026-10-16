---
title: "CellFilter"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Fornisce un'opzione per limitare l'ambito di una CellColumnRedaction a un foglio di lavoro e a una colonna."
type: docs
weight: 12
url: /it/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

Fornisce un'opzione per limitare l'ambito di un
CellColumnRedaction
a un foglio di lavoro e a una colonna.

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | Inizializza una nuova istanza. |
|
## Campi

| Campo | Descrizione |
| --- | --- |
|  | [NoIndex](#NoIndex) | Rappresenta un valore predefinito per il filtro, che è -1. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | Ottiene il nome del foglio di lavoro (se applicabile). |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | Imposta il nome del foglio di lavoro (se applicabile). |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | Ottiene l'indice del foglio di lavoro (basato su zero). |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | Imposta l'indice del foglio di lavoro (basato su zero). |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | Ottiene un valore che indica se il |
WorkSheetIndex
è impostato o meno.
|
|  | [getColumnIndex()](#getColumnIndex--) | Ottiene un indice di colonna (basato su zero). |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | Imposta un indice di colonna (basato su zero). |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


Inizializza una nuova istanza.


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


Rappresenta un valore predefinito per il filtro, che è -1.


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


Ottiene il nome del foglio di lavoro (se applicabile).


**Returns:**
java.lang.String - Un nome di foglio di lavoro (se applicabile).

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


Imposta il nome del foglio di lavoro (se applicabile).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Un nome di foglio di lavoro (se applicabile). |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


Ottiene l'indice del foglio di lavoro (basato su zero).


**Returns:**
int - Un indice di foglio di lavoro (basato su zero).

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


Imposta l'indice del foglio di lavoro (basato su zero).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Un indice di foglio di lavoro (basato su zero). |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


Ottiene un valore che indica se il
WorkSheetIndex
è impostato o meno.


**Returns:**
boolean - Un valore che indica se il  WorkSheetIndex  è impostato o meno.

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


Ottiene un indice di colonna (basato su zero).


**Returns:**
int - Un indice di colonna (basato su zero).

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


Imposta un indice di colonna (basato su zero).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Un indice di colonna (basato su zero). |
|

