---
title: "Redactor"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示一个主要类，控制文档编辑过程，允许打开、编辑并保存文档。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

表示控制文档编辑过程的主类，允许打开、编辑和保存文档。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | 初始化一个新实例 |
Redactor
使用文件路径的类。
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | 初始化一个新实例 |
Redactor
使用流的类。
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | 初始化一个新实例 |
Redactor
使用路径的受密码保护文档的类。
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | 初始化一个新实例 |
Redactor
使用路径和设置的受密码保护文档的类。
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | 初始化一个新实例 |
Redactor
使用流的受密码保护文档的类。
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | 初始化一个新实例 |
Redactor
使用流和设置的受密码保护文档的类。
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [close()](#close--) | 释放资源。 |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | 对文档应用编辑。 |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | 对文档应用一组编辑。 |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | 对文档应用编辑策略。 |
|
|  | [save()](#save--) | 将文档保存到文件，并使用以下选项：AddSuffix = true，RasterizeToPDF = true。 |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | 将文档保存到文件。 |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | 将文档保存到流。 |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | 将文档保存到流。 |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | 将文档保存到流，包括自定义位置。 |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | 生成特定页面的预览图像，使用给定的图像格式。 |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | 获取文档的一般信息——大小、页数等。 |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


初始化一个新实例
Redactor
使用文件路径的类。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件路径 |


以下示例演示如何打开文档进行编辑。

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
     // Here we can use document instance to perform redactions
 }
 
``` 
````

 |

### Redactor(InputStream document) {#Redactor-java.io.InputStream-}
```
public Redactor(InputStream document)
```


Initializes a new instance of 
Redactor
 class using stream.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source stream of the document


The following example demonstrates how to open a document from stream.

````

try (InputStream stream = new FileInputStream("C:\\sample.pdf"))
{
try (Redactor redactor = new Redactor(stream))
{
// 在这里我们可以使用文档实例执行编辑
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


初始化一个新实例
Redactor
使用路径的受密码保护文档的类。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件路径。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | 选项，包括密码。 |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


初始化一个新实例
Redactor
使用路径和设置的受密码保护文档的类。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件路径。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | 文件相关选项，包括密码。 |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | 编辑过程的默认设置。 |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


初始化一个新实例
Redactor
使用流的受密码保护文档的类。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档 | java.io.InputStream | 源输入流。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | 选项，包括密码。 |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


初始化一个新实例
Redactor
使用流和设置的受密码保护文档的类。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档 | java.io.InputStream | 源输入流。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | 选项，包括密码。 |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | 编辑过程的默认设置。 |
|

### close() {#close--}
```
public final void close()
```


释放资源。


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


对文档应用编辑。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | 要应用的  Redaction  实例 |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


对文档应用一组编辑。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | 要应用的编辑数组 |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


对文档应用编辑策略。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | 编辑策略 |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


将文档保存到文件，并使用以下选项：AddSuffix = true，RasterizeToPDF = true。


**Returns:**
java.lang.String - 已编辑文档的路径

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


将文档保存到文件。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | 添加后缀或光栅化的选项 |
|

**Returns:**
java.lang.String - 已编辑文档的路径

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


将文档保存到流。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档 | java.io.OutputStream | 目标流 |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


将文档保存到流。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档 | java.io.OutputStream | 目标流 |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | 保存选项 |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


将文档保存到流，包括自定义位置。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档 | java.io.OutputStream | 目标流 |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | 是否光栅化以及指定光栅化页面的选项 |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


生成特定页面的预览图像，使用给定的图像格式。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | 图像属性和页面范围设置 |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


获取文档的一般信息——大小、页数等。


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

