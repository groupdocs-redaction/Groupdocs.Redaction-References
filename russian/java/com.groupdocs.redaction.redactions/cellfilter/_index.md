---
title: "CellFilter"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Предоставляет параметр для ограничения области действия CellColumnRedaction листом и столбцом."
type: docs
weight: 12
url: /ru/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

Предоставляет возможность ограничить область
CellColumnRedaction
для листа и столбца.

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | Инициализирует новый экземпляр. |
|
## Поля

| Поле | Описание |
| --- | --- |
|  | [NoIndex](#NoIndex) | Представляет значение по умолчанию для фильтра, которое равно -1. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | Получает имя листа (если применимо). |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | Устанавливает имя листа (если применимо). |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | Получает индекс листа (нумерация с нуля). |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | Устанавливает индекс листа (нумерация с нуля). |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | Получает значение, указывающее, является ли |
WorkSheetIndex
установлен или нет.
|
|  | [getColumnIndex()](#getColumnIndex--) | Получает индекс столбца (нумерация с нуля). |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | Устанавливает индекс столбца (нумерация с нуля). |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


Инициализирует новый экземпляр.


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


Представляет значение по умолчанию для фильтра, которое равно -1.


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


Получает имя листа (если применимо).


**Returns:**
java.lang.String — имя листа (если применимо).

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


Устанавливает имя листа (если применимо).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Имя листа (если применимо). |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


Получает индекс листа (нумерация с нуля).


**Returns:**
int — индекс листа (нумерация с нуля).

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


Устанавливает индекс листа (нумерация с нуля).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Индекс листа (нумерация с нуля). |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


Получает значение, указывающее, является ли
WorkSheetIndex
установлен или нет.


**Returns:**
boolean — значение, указывающее, установлен ли WorkSheetIndex или нет.

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


Получает индекс столбца (нумерация с нуля).


**Returns:**
int — индекс столбца (нумерация с нуля).

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


Устанавливает индекс столбца (нумерация с нуля).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Индекс столбца (нумерация с нуля). |
|

