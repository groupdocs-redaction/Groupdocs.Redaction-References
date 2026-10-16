---
title: "CellFilter"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "提供将 CellColumnRedaction 的范围限制在工作表和列的选项。"
type: docs
weight: 12
url: /zh/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

提供一个选项以限制范围。
CellColumnRedaction
到工作表和列。

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | 初始化新实例。 |
|
## 字段

| 字段 | 描述 |
| --- | --- |
|  | [NoIndex](#NoIndex) | 表示过滤器的默认值，为 -1。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | 获取工作表名称（如果适用）。 |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | 设置工作表名称（如果适用）。 |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | 获取工作表索引（从零开始）。 |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | 设置工作表索引（从零开始）。 |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | 获取指示是否的值。 |
WorkSheetIndex
是否已设置。
|
|  | [getColumnIndex()](#getColumnIndex--) | 获取列索引（从零开始）。 |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | 设置列索引（从零开始）。 |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


初始化新实例。


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


表示过滤器的默认值，为 -1。


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


获取工作表名称（如果适用）。


**Returns:**
java.lang.String - 工作表名称（如适用）。

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


设置工作表名称（如果适用）。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 工作表名称（如适用）。 |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


获取工作表索引（从零开始）。


**Returns:**
int - 工作表索引（从零开始）。

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


设置工作表索引（从零开始）。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 工作表索引（从零开始）。 |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


获取指示是否的值。
WorkSheetIndex
是否已设置。


**Returns:**
boolean - 一个值，指示 WorkSheetIndex 是否已设置。

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


获取列索引（从零开始）。


**Returns:**
int - 列索引（从零开始）。

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


设置列索引（从零开始）。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 列索引（从零开始）。 |
|

