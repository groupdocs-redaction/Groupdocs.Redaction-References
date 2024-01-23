---
title: CellFilter
second_title: GroupDocs.Redaction for Java API Reference
description: Provides an option to limit the scope of a CellColumnRedaction to a worksheet and a column.
type: docs
weight: 12
url: /java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

Provides an option to limit the scope of a  CellColumnRedaction  to a worksheet and a column.

--------------------

**Learn more**

 *  More details about spreadsheet redactions: [Spreadsheet redactions][]


[Spreadsheet redactions]: https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/
## Constructors

| Constructor | Description |
| --- | --- |
| [CellFilter()](#CellFilter--) | Initializes a new instance. |
## Fields

| Field | Description |
| --- | --- |
| [NoIndex](#NoIndex) | Represents a default value for filter, which is -1. |
## Methods

| Method | Description |
| --- | --- |
| [getWorkSheetName()](#getWorkSheetName--) | Gets a worksheet name (if applicable). |
| [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | Sets a worksheet name (if applicable). |
| [getWorkSheetIndex()](#getWorkSheetIndex--) | Gets a worksheet index (zero-based). |
| [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | Sets a worksheet index (zero-based). |
| [hasWorkSheetIndex()](#hasWorkSheetIndex--) | Gets a value indicating whether the  WorkSheetIndex  is set or not. |
| [getColumnIndex()](#getColumnIndex--) | Gets a column index (zero-based). |
| [setColumnIndex(int value)](#setColumnIndex-int-) | Sets a column index (zero-based). |
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


Initializes a new instance.

### NoIndex {#NoIndex}
```
public static final int NoIndex
```


Represents a default value for filter, which is -1.

### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


Gets a worksheet name (if applicable).

**Returns:**
java.lang.String - A worksheet name (if applicable).
### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


Sets a worksheet name (if applicable).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | A worksheet name (if applicable). |

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


Gets a worksheet index (zero-based).

**Returns:**
int - A worksheet index (zero-based).
### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


Sets a worksheet index (zero-based).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | A worksheet index (zero-based). |

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


Gets a value indicating whether the  WorkSheetIndex  is set or not.

**Returns:**
boolean - A value indicating whether the  WorkSheetIndex  is set or not.
### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


Gets a column index (zero-based).

**Returns:**
int - A column index (zero-based).
### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


Sets a column index (zero-based).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | A column index (zero-based). |

