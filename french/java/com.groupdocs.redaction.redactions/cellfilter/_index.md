---
title: "CellFilter"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Fournit une option pour limiter la portée d'une CellColumnRedaction à une feuille de calcul et à une colonne."
type: docs
weight: 12
url: /fr/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

Fournit une option pour limiter la portée d'un
CellColumnRedaction
à une feuille de calcul et à une colonne.

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | Initialise une nouvelle instance. |
|
## Champs

| Champ | Description |
| --- | --- |
|  | [NoIndex](#NoIndex) | Représente une valeur par défaut pour le filtre, qui est -1. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | Obtient le nom d'une feuille de calcul (le cas échéant). |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | Définit le nom d'une feuille de calcul (le cas échéant). |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | Obtient l'index d'une feuille de calcul (à base zéro). |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | Définit l'index d'une feuille de calcul (à base zéro). |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | Obtient une valeur indiquant si le |
WorkSheetIndex
est défini ou non.
|
|  | [getColumnIndex()](#getColumnIndex--) | Obtient un indice de colonne (à partir de zéro). |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | Définit un indice de colonne (à partir de zéro). |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


Initialise une nouvelle instance.


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


Représente une valeur par défaut pour le filtre, qui est -1.


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


Obtient le nom d'une feuille de calcul (le cas échéant).


**Returns:**
java.lang.String - Un nom de feuille de calcul (le cas échéant).

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


Définit le nom d'une feuille de calcul (le cas échéant).


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | Un nom de feuille de calcul (le cas échéant). |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


Obtient l'index d'une feuille de calcul (à base zéro).


**Returns:**
int - Un indice de feuille de calcul (à partir de zéro).

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


Définit l'index d'une feuille de calcul (à base zéro).


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Un indice de feuille de calcul (à partir de zéro). |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


Obtient une valeur indiquant si le
WorkSheetIndex
est défini ou non.


**Returns:**
boolean - Une valeur indiquant si le  WorkSheetIndex  est défini ou non.

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


Obtient un indice de colonne (à partir de zéro).


**Returns:**
int - Un indice de colonne (à partir de zéro).

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


Définit un indice de colonne (à partir de zéro).


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Un indice de colonne (à partir de zéro). |
|

