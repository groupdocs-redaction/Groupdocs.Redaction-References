---
title: "CellFilter"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Bietet eine Option, den Geltungsbereich einer CellColumnRedaction auf ein Arbeitsblatt und eine Spalte zu beschränken."
type: docs
weight: 12
url: /de/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

Bietet eine Option, den Geltungsbereich einer
CellColumnRedaction
zu einem Arbeitsblatt und einer Spalte.

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | Initialisiert eine neue Instanz. |
|
## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [NoIndex](#NoIndex) | Stellt einen Standardwert für den Filter dar, der -1 ist. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | Liest einen Arbeitsblattnamen (falls zutreffend). |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | Setzt einen Arbeitsblattnamen (falls zutreffend). |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | Liest einen Arbeitsblattindex (nullbasiert). |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | Setzt einen Arbeitsblattindex (nullbasiert). |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | Liest einen Wert, der angibt, ob das |
WorkSheetIndex
gesetzt ist oder nicht.
|
|  | [getColumnIndex()](#getColumnIndex--) | Liest einen Spaltenindex (nullbasiert). |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | Setzt einen Spaltenindex (nullbasiert). |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


Initialisiert eine neue Instanz.


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


Stellt einen Standardwert für den Filter dar, der -1 ist.


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


Liest einen Arbeitsblattnamen (falls zutreffend).


**Returns:**
java.lang.String - Ein Arbeitsblattname (falls zutreffend).

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


Setzt einen Arbeitsblattnamen (falls zutreffend).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Ein Arbeitsblattname (falls zutreffend). |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


Liest einen Arbeitsblattindex (nullbasiert).


**Returns:**
int - Ein Arbeitsblattindex (nullbasiert).

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


Setzt einen Arbeitsblattindex (nullbasiert).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Ein Arbeitsblattindex (nullbasiert). |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


Liest einen Wert, der angibt, ob das
WorkSheetIndex
gesetzt ist oder nicht.


**Returns:**
boolean - Ein Wert, der angibt, ob der  WorkSheetIndex  gesetzt ist oder nicht.

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


Liest einen Spaltenindex (nullbasiert).


**Returns:**
int - Ein Spaltenindex (nullbasiert).

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


Setzt einen Spaltenindex (nullbasiert).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Ein Spaltenindex (nullbasiert). |
|

