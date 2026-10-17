---
title: "MetadataItem"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثّل عنصر بيانات وصفية مشترك لجميع التنسيقات المدعومة ويُستخدم في تعديل البيانات الوصفية."
type: docs
weight: 12
url: /ar/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

يمثل عنصرًا من البيانات الوصفية، شائعًا لجميع الصيغ المدعومة ويُستخدم في تعديل البيانات الوصفية.

## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | يقوم بإنشاء نسخة جديدة. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | يحصل على الاسم الأصلي لعنصر البيانات الوصفية كما يظهر في المستند. |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | يضبط الاسم الأصلي لعنصر البيانات الوصفية كما يظهر في المستند. |
|
|  | [getCategory()](#getCategory--) | يحصل على فئة عنصر البيانات الوصفية، على سبيل المثال معرف المورد لعنصر بيانات وصفية مورد مدمج. |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | يضبط فئة عنصر البيانات الوصفية، على سبيل المثال معرف المورد لعنصر بيانات وصفية مدمج. |
|
|  | [getFilter()](#getFilter--) | يحصل على قيمة من |
MetadataFilters
، مخصص لهذا العنصر الوصفي والذي يُستخدم في تصفية العناصر.
|
|  | [setFilter(int value)](#setFilter-int-) | يضبط قيمة من |
MetadataFilters
، مخصص لهذا العنصر الوصفي والذي يُستخدم في تصفية العناصر.
|
|  | [getValues()](#getValues--) | يحصل على قيمة عنصر البيانات الوصفية. |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | يضبط قيمة عنصر البيانات الوصفية. |
|
|  | [isCustom()](#isCustom--) | يحصل على قيمة تشير إلى ما إذا كان هذا العنصر مخصصًا (أضيف من قبل مؤلفي المستند). |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | يضبط قيمة تشير إلى ما إذا كان هذا العنصر مخصصًا (أضيف من قبل مؤلفي المستند). |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | يحصل على مفتاح القاموس لـ , باستخدام اسمه الأصلي وبيانات أخرى. |
|
|  | [createClone()](#createClone--) | ينشئ نسخة عميقة من المثيل الحالي. |
|
|  | [getActualValue()](#getActualValue--) | يحصل على التمثيل النصي لقيمة عنصر البيانات الوصفية. |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


يقوم بإنشاء نسخة جديدة.


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


يحصل على الاسم الأصلي لعنصر البيانات الوصفية كما يظهر في المستند.


**Returns:**
java.lang.String - اسم أصلي لعنصر البيانات الوصفية كما يظهر في المستند.

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


يضبط الاسم الأصلي لعنصر البيانات الوصفية كما يظهر في المستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.lang.String | اسم أصلي لعنصر البيانات الوصفية كما يظهر في المستند. |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


يحصل على فئة عنصر البيانات الوصفية، على سبيل المثال معرف المورد لعنصر بيانات وصفية مورد مدمج.


**Returns:**
java.lang.String - فئة عنصر البيانات الوصفية، على سبيل المثال معرف المورد لعنصر بيانات وصفية مدمج.

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


يضبط فئة عنصر البيانات الوصفية، على سبيل المثال معرف المورد لعنصر بيانات وصفية مدمج.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.lang.String | فئة عنصر البيانات الوصفية، على سبيل المثال معرف المورد لعنصر بيانات وصفية مدمج. |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


يحصل على قيمة من
MetadataFilters
، مخصص لهذا العنصر الوصفي والذي يُستخدم في تصفية العناصر.


**Returns:**
int - قيمة من  MetadataFilters , مخصصة لهذا عنصر البيانات الوصفية والذي يُستخدم في تصفية العناصر.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


يضبط قيمة من
MetadataFilters
، مخصص لهذا العنصر الوصفي والذي يُستخدم في تصفية العناصر.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | int | قيمة من  MetadataFilters , مخصصة لهذا عنصر البيانات الوصفية والذي يُستخدم في تصفية العناصر. |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


يحصل على قيمة عنصر البيانات الوصفية.


**Returns:**
java.util.List<java.lang.String> - قيمة عنصر البيانات الوصفية.

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


يضبط قيمة عنصر البيانات الوصفية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.util.List<java.lang.String> | قيمة عنصر البيانات الوصفية. |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


يحصل على قيمة تشير إلى ما إذا كان هذا العنصر مخصصًا (أضيف من قبل مؤلفي المستند).


**Returns:**
boolean - قيمة تشير إلى ما إذا كان هذا العنصر مخصصًا (أضيف من قبل مؤلفي المستند).

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان هذا العنصر مخصصًا (أضيف من قبل مؤلفي المستند).


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | boolean | قيمة تشير إلى ما إذا كان هذا العنصر مخصصًا (أضيف من قبل مؤلفي المستند). |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


يحصل على مفتاح القاموس لـ , باستخدام اسمه الأصلي وبيانات أخرى.


**Returns:**
java.lang.String - مفتاح القاموس لـ , باستخدام اسمه الأصلي وبيانات أخرى.

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


ينشئ نسخة عميقة من المثيل الحالي.


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


يحصل على التمثيل النصي لقيمة عنصر البيانات الوصفية.


**Returns:**
java.lang.String - التمثيل النصي لقيمة عنصر البيانات الوصفية.

