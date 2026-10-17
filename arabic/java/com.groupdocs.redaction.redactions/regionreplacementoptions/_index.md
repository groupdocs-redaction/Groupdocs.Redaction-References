---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل معلمات اللون والمساحة لاستبدال منطقة الصورة."
type: docs
weight: 29
url: /ar/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

يمثل معلمات اللون والمساحة لاستبدال منطقة الصورة. راجع
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | ينشئ مثيلًا جديدًا لفئة RegionReplacementOptions. |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | ينشئ مثيلًا جديدًا لفئة RegionReplacementOptions حيث يتطابق الحجم مع النص المعطى. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | يحصل على اللون لملء المنطقة المخفية. |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | يضبط اللون لملء المنطقة المخفية. |
|
|  | [getSize()](#getSize--) | يحصل على المستطيل بالعرض والارتفاع. |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | يضبط المستطيل بالعرض والارتفاع. |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


ينشئ مثيلًا جديدًا لفئة RegionReplacementOptions.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | fillColor | java.awt.Color | اللون لملء المنطقة |
|
|  | size | java.awt.Dimension | حجم المنطقة المملوءة |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


ينشئ مثيلًا جديدًا لفئة RegionReplacementOptions حيث يتطابق الحجم مع النص المعطى.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | fillColor | java.awt.Color | اللون لملء المنطقة |
|
|  | font | java.awt.Font | خط النص المتوقع |
|
|  | expectedText | java.lang.String | النص المتوقع |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


يحصل على اللون لملء المنطقة المخفية.


**Returns:**
java.awt.Color - اللون لملء المنطقة المحذوفة.

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


يضبط اللون لملء المنطقة المخفية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.awt.Color | اللون لملء المنطقة المحذوفة. |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


يحصل على المستطيل بالعرض والارتفاع.


**Returns:**
java.awt.Dimension - المستطيل بالعرض والارتفاع.

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


يضبط المستطيل بالعرض والارتفاع.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.awt.Dimension | المستطيل بالعرض والارتفاع. |
|

