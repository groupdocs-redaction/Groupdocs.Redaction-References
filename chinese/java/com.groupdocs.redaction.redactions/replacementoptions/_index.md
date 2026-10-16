---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示匹配文本替换的选项。"
type: docs
weight: 31
url: /zh/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

表示匹配文本替换的选项。

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | 使用替换文本作为选项初始化 ReplacementOptions 类的新实例。 |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | 使用彩色矩形作为选项初始化 ReplacementOptions 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getActionType()](#getActionType--) | 获取替换操作：绘制框或替换文本。 |
|
|  | [getReplacement()](#getReplacement--) | 获取文本替换值。 |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | 设置文本替换值。 |
|
|  | [getBoxColor()](#getBoxColor--) | 获取 a 的颜色 |
ReplacementType.DrawBox
选项（在其他情况下被忽略）。
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | 设置颜色用于 |
ReplacementType.DrawBox
选项（在其他情况下被忽略）。
|
|  | [getFilters()](#getFilters--) | 获取用于此编辑的过滤器数组。 |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | 设置用于此编辑的过滤器数组。 |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | 获取自定义编辑处理程序。 |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | 设置自定义编辑处理程序。 |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


使用替换文本作为选项初始化 ReplacementOptions 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 替换 | java.lang.String | 文本替换 |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


使用彩色矩形作为选项初始化 ReplacementOptions 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 颜色 | java.awt.Color | 矩形颜色 |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


获取替换操作：绘制框或替换文本。


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


获取文本替换值。


**Returns:**
java.lang.String - 文本替换值。

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


设置文本替换值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 文本替换值。 |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


获取 a 的颜色
ReplacementType.DrawBox
选项（在其他情况下被忽略）。


**Returns:**
java.awt.Color - 用于  ReplacementType.DrawBox  选项的颜色（在其他情况下被忽略）。

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


设置颜色用于
ReplacementType.DrawBox
选项（在其他情况下被忽略）。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.awt.Color | 用于  ReplacementType.DrawBox  选项的颜色（在其他情况下被忽略）。 |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


获取用于此编辑的过滤器数组。


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - 用于此编辑的过滤器数组。

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


设置用于此编辑的过滤器数组。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | 用于此编辑的过滤器数组。 |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


获取自定义编辑处理程序。仅支持 PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction)。


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


设置自定义编辑处理程序。仅支持 PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction)。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) 的实例。 |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
