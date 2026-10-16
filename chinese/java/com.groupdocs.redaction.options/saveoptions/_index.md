---
title: "SaveOptions"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "提供更改输出文件名和/或将文档转换为基于图像的 PDF 光栅化的选项。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

提供更改输出文件名和/或将文档转换为基于图像的 PDF（光栅化）的选项。

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | 使用默认值初始化新实例：光栅化为 PDF - false，添加后缀 - false。 |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | 使用给定参数初始化新实例。 |
|
## 字段

| 字段 | 描述 |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | 表示默认后缀值，为 "Redacted"。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | 获取一个值，指示在保存之前是否需要更改文件名。 |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | 设置一个值，指示在保存之前是否需要更改文件名。 |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | 获取输出文件名的自定义后缀。 |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | 设置输出文件名的自定义后缀。 |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | 获取一个值，指示文档中的所有页面是否需要转换为图像并放入单个 PDF 文件。 |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | 设置一个值，指示文档中的所有页面是否需要转换为图像并放入单个 PDF 文件。 |
|
|  | [getRasterization()](#getRasterization--) | 获取光栅化设置。 |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | 文字处理保存选项。 |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


使用默认值初始化新实例：光栅化为 PDF - false，添加后缀 - false。


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


使用给定参数初始化新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | 如果文档中的所有页面需要转换为图像并放入单个 PDF 文件，则为 True |
|
|  | suffix | java.lang.String | 此文本将添加到文件名末尾，如果不为空，还会将 AddSuffix 设置为 true |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


表示默认后缀值，为 "Redacted"。


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


获取一个值，指示在保存之前是否需要更改文件名。默认值为 False。


**Returns:**
boolean - 一个值，指示在保存之前是否需要更改文件名。默认值为 False。

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


设置一个值，指示在保存之前是否需要更改文件名。默认值为 False。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 一个值，指示在保存之前是否需要更改文件名。默认值为 False。 |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


获取输出文件名的自定义后缀。如果未指定，则
SaveSuffix
常量将被使用。


**Returns:**
java.lang.String - 输出文件名的自定义后缀。如果未指定，则使用  SaveSuffix  常量。

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


设置输出文件名的自定义后缀。如果未指定，则
SaveSuffix
常量将被使用。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 用于输出文件名的自定义后缀。如果未指定，将使用 SaveSuffix 常量。 |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


获取一个值，指示文档中的所有页面是否需要转换为图像并放入单个 PDF 文件。


**Returns:**
boolean - 一个指示文档中所有页面是否需要转换为图像并放入单个 PDF 文件的值。

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


设置一个值，指示文档中的所有页面是否需要转换为图像并放入单个 PDF 文件。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 一个指示文档中所有页面是否需要转换为图像并放入单个 PDF 文件的值。 |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


获取光栅化设置。


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


文字处理保存选项。


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
