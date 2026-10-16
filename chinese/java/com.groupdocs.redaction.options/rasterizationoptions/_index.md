---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "提供将文件转换为 PDF 的选项。"
type: docs
weight: 12
url: /zh/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

提供将文件转换为 PDF 的选项。

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | 初始化新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | 获取一个值，指示文档中的所有页面是否需要转换为图像并放入单个 PDF 文件。 |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | 设置一个值，指示文档中的所有页面是否需要转换为图像并放入单个 PDF 文件。 |
|
|  | [getPageIndex()](#getPageIndex--) | 获取要转换为 PDF 的第一页（基于 0）的索引。 |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | 设置要转换为 PDF 的第一页（基于 0）的索引。 |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | 获取一个值，指示在初始化后 PageIndex 属性是否已更改（设置）。 |
|
|  | [getPageCount()](#getPageCount--) | 获取要转换为 PDF 的页数。 |
|
|  | [setPageCount(int value)](#setPageCount-int-) | 设置要转换为 PDF 的页数。 |
|
|  | [isPageCountSet()](#isPageCountSet--) | 获取一个值，指示在初始化后 PageCount 属性是否已更改（设置）。 |
|
|  | [getCompliance()](#getCompliance--) | 获取 PDF 合规级别。 |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | 设置 PDF 合规级别。 |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | 获取指示器，如果已设置高级光栅化选项则为 true。 |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | 您可以使用此方法注册要应用的高级光栅化选项。 |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | 您可以使用此方法注册要应用的高级光栅化选项。 |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


初始化新实例。


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


获取一个值，指示文档中的所有页面是否需要转换为图像并放入单个 PDF 文件。默认 TRUE，若要避免光栅化请设为 FALSE。


**Returns:**
boolean - 一个值，指示文档中的所有页面是否需要转换为图像并放入单个 PDF 文件。默认 TRUE，若要避免光栅化请设为 FALSE。

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


设置一个值，指示文档中的所有页面是否需要转换为图像并放入单个 PDF 文件。默认 TRUE，若要避免光栅化请设为 FALSE。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 一个值，指示文档中的所有页面是否需要转换为图像并放入单个 PDF 文件。默认 TRUE，若要避免光栅化请设为 FALSE。 |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


获取要转换为 PDF 的第一页（基于 0）的索引。


**Returns:**
int - 要转换为 PDF 的第一页（从 0 开始计数）的索引。

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


设置要转换为 PDF 的第一页（基于 0）的索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 要转换为 PDF 的第一页（从 0 开始计数）的索引。 |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


获取一个值，指示在初始化后 PageIndex 属性是否已更改（设置）。


**Returns:**
boolean - 一个值，指示在初始化后 PageIndex 属性是否已更改（设置）。

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


获取要转换为 PDF 的页数。


**Returns:**
int - 要转换为 PDF 的页数。

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


设置要转换为 PDF 的页数。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 要转换为 PDF 的页数。 |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


获取一个值，指示在初始化后 PageCount 属性是否已更改（设置）。


**Returns:**
boolean - 一个值，指示在初始化后 PageCount 属性是否已更改（设置）。

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


获取 PDF 合规级别。


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


设置 PDF 合规级别。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | PDF 合规级别。 |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


获取指示器，如果已设置高级光栅化选项则为 true。


**Returns:**
boolean - 一个指示器，如果已设置高级光栅化选项则为 true。

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


您可以使用此方法注册要应用的高级光栅化选项。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | 提供有关所选效果类型（灰度、边框等）的信息。 |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


您可以使用此方法注册要应用的高级光栅化选项。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | 提供有关所选效果类型（灰度、边框等）的信息。 |
|
|  | 参数 | java.util.HashMap<java.lang.String,java.lang.String> | 给定效果的参数，例如旋转角度 |
|

