---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示图像区域替换的颜色和区域参数。"
type: docs
weight: 29
url: /zh/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

表示图像区域替换的颜色和区域参数。参见
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | 初始化 RegionReplacementOptions 类的新实例。 |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | 初始化 RegionReplacementOptions 类的新实例，其大小匹配给定文本。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | 获取用于填充编辑区域的颜色。 |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | 设置用于填充编辑区域的颜色。 |
|
|  | [getSize()](#getSize--) | 获取矩形的宽度和高度。 |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | 设置矩形的宽度和高度。 |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


初始化 RegionReplacementOptions 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fillColor | java.awt.Color | 用于填充区域的颜色 |
|
|  | 大小 | java.awt.Dimension | 已填充区域的大小 |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


初始化 RegionReplacementOptions 类的新实例，其大小匹配给定文本。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fillColor | java.awt.Color | 用于填充区域的颜色 |
|
|  | font | java.awt.Font | 期望的文本字体 |
|
|  | expectedText | java.lang.String | 期望的文本 |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


获取用于填充编辑区域的颜色。


**Returns:**
java.awt.Color - 用于填充已编辑区域的颜色。

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


设置用于填充编辑区域的颜色。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.awt.Color | 用于填充已编辑区域的颜色。 |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


获取矩形的宽度和高度。


**Returns:**
java.awt.Dimension - 矩形的宽度和高度。

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


设置矩形的宽度和高度。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.awt.Dimension | 矩形的宽度和高度。 |
|

