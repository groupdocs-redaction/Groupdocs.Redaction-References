---
title: "CellFilter"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يوفر خيارًا لتحديد نطاق CellColumnRedaction إلى ورقة عمل وعمود."
type: docs
weight: 12
url: /ar/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

يوفر خيارًا لتقييد نطاق
CellColumnRedaction
إلى ورقة عمل وعمود.

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | يقوم بإنشاء نسخة جديدة. |
|
## الحقول

| حقل | الوصف |
| --- | --- |
|  | [NoIndex](#NoIndex) | يمثل القيمة الافتراضية للمرشح، والتي هي -1. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | يحصل على اسم ورقة العمل (إن وجد). |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | يضبط اسم ورقة العمل (إن وجد). |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | يحصل على فهرس ورقة العمل (بدءًا من الصفر). |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | يضبط فهرس ورقة العمل (بدءًا من الصفر). |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | يحصل على قيمة تشير إلى ما إذا كان |
WorkSheetIndex
مُعين أو غير مُعين.
|
|  | [getColumnIndex()](#getColumnIndex--) | يحصل على فهرس العمود (مبني على الصفر). |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | يضبط فهرس العمود (مبني على الصفر). |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


يقوم بإنشاء نسخة جديدة.


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


يمثل القيمة الافتراضية للمرشح، والتي هي -1.


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


يحصل على اسم ورقة العمل (إن وجد).


**Returns:**
java.lang.String - اسم ورقة العمل (إن وجد).

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


يضبط اسم ورقة العمل (إن وجد).


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.lang.String | اسم ورقة العمل (إن وجد). |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


يحصل على فهرس ورقة العمل (بدءًا من الصفر).


**Returns:**
int - فهرس ورقة العمل (مبني على الصفر).

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


يضبط فهرس ورقة العمل (بدءًا من الصفر).


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | int | فهرس ورقة العمل (مبني على الصفر). |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


يحصل على قيمة تشير إلى ما إذا كان
WorkSheetIndex
مُعين أو غير مُعين.


**Returns:**
boolean - قيمة تشير إلى ما إذا كان WorkSheetIndex مُعينًا أم لا.

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


يحصل على فهرس العمود (مبني على الصفر).


**Returns:**
int - فهرس العمود (مبني على الصفر).

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


يضبط فهرس العمود (مبني على الصفر).


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | int | فهرس العمود (مبني على الصفر). |
|

