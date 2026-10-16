---
title: "MetadataItem"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示所有受支持格式通用的元数据项，并用于元数据编辑。"
type: docs
weight: 12
url: /zh/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

表示元数据项，适用于所有受支持的格式，并用于元数据编辑。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | 初始化新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | 获取元数据项在文档中出现的原始名称。 |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | 设置元数据项在文档中出现的原始名称。 |
|
|  | [getCategory()](#getCategory--) | 获取元数据项的类别，例如嵌入资源元数据项的资源 ID。 |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | 设置元数据项的类别，例如嵌入资源元数据项的资源 ID。 |
|
|  | [getFilter()](#getFilter--) | 获取一个值的 |
MetadataFilters
，分配给此元数据项，用于项目过滤。
|
|  | [setFilter(int value)](#setFilter-int-) | 设置一个值的 |
MetadataFilters
，分配给此元数据项，用于项目过滤。
|
|  | [getValues()](#getValues--) | 获取元数据项的值。 |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | 设置元数据项的值。 |
|
|  | [isCustom()](#isCustom--) | 获取一个值，指示此项是否为自定义（由文档作者添加）。 |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | 设置一个值，指示此项是否为自定义（由文档作者添加）。 |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | 获取字典键，用于 ，使用其 OriginalName 和其他数据。 |
|
|  | [createClone()](#createClone--) | 创建当前实例的深度克隆。 |
|
|  | [getActualValue()](#getActualValue--) | 获取元数据项值的字符串表示形式。 |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


初始化新实例。


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


获取元数据项在文档中出现的原始名称。


**Returns:**
java.lang.String - 元数据项的原始名称，出现在文档中。

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


设置元数据项在文档中出现的原始名称。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 元数据项的原始名称，出现在文档中。 |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


获取元数据项的类别，例如嵌入资源元数据项的资源 ID。


**Returns:**
java.lang.String - 元数据项的类别，例如嵌入资源元数据项的资源 ID。

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


设置元数据项的类别，例如嵌入资源元数据项的资源 ID。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 元数据项的类别，例如嵌入资源元数据项的资源 ID。 |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


获取一个值的
MetadataFilters
，分配给此元数据项，用于项目过滤。


**Returns:**
int - MetadataFilters 的一个值，分配给此元数据项，用于项目过滤。

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


设置一个值的
MetadataFilters
，分配给此元数据项，用于项目过滤。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | MetadataFilters 的一个值，分配给此元数据项，用于项目过滤。 |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


获取元数据项的值。


**Returns:**
java.util.List<java.lang.String> - 元数据项的值。

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


设置元数据项的值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.util.List<java.lang.String> | 元数据项的值。 |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


获取一个值，指示此项是否为自定义（由文档作者添加）。


**Returns:**
boolean - 一个值，指示此项是否为自定义（由文档作者添加）。

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


设置一个值，指示此项是否为自定义（由文档作者添加）。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 一个值，指示此项是否为自定义（由文档作者添加）。 |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


获取字典键，用于 ，使用其 OriginalName 和其他数据。


**Returns:**
java.lang.String - 一个字典键，用于 ，使用其 OriginalName 和其他数据。

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


创建当前实例的深度克隆。


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


获取元数据项值的字符串表示形式。


**Returns:**
java.lang.String - 元数据项值的字符串表示形式。

