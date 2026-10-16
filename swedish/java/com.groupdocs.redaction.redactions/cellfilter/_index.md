---
title: "CellFilter"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Tillhandahåller ett alternativ för att begränsa omfattningen av en CellColumnRedaction till ett arbetsblad och en kolumn."
type: docs
weight: 12
url: /sv/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

Tillhandahåller ett alternativ för att begränsa omfattningen av en
CellColumnRedaction
till ett kalkylblad och en kolumn.

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | Initierar en ny instans. |
|
## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [NoIndex](#NoIndex) | Representerar ett standardvärde för filtret, vilket är -1. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | Hämtar ett kalkylbladsnamn (om tillämpligt). |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | Ställer in ett kalkylbladsnamn (om tillämpligt). |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | Hämtar ett kalkylbladsindex (nollbaserat). |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | Ställer in ett kalkylbladsindex (nollbaserat). |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | Hämtar ett värde som indikerar om |
WorkSheetIndex
är satt eller inte.
|
|  | [getColumnIndex()](#getColumnIndex--) | Hämtar ett kolumnindex (nollbaserat). |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | Ställer in ett kolumnindex (nollbaserat). |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


Initierar en ny instans.


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


Representerar ett standardvärde för filtret, vilket är -1.


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


Hämtar ett kalkylbladsnamn (om tillämpligt).


**Returns:**
java.lang.String - Ett arbetsbladsnamn (om tillämpligt).

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


Ställer in ett kalkylbladsnamn (om tillämpligt).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Ett arbetsbladsnamn (om tillämpligt). |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


Hämtar ett kalkylbladsindex (nollbaserat).


**Returns:**
int - Ett arbetsbladsindex (nollbaserat).

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


Ställer in ett kalkylbladsindex (nollbaserat).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Ett arbetsbladsindex (nollbaserat). |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


Hämtar ett värde som indikerar om
WorkSheetIndex
är satt eller inte.


**Returns:**
boolean - Ett värde som indikerar om  WorkSheetIndex  är satt eller inte.

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


Hämtar ett kolumnindex (nollbaserat).


**Returns:**
int - Ett kolumnindex (nollbaserat).

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


Ställer in ett kolumnindex (nollbaserat).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Ett kolumnindex (nollbaserat). |
|

