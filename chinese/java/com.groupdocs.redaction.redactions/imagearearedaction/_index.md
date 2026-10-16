---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示一种编辑，在图像文档的指定区域放置彩色矩形。"
type: docs
weight: 18
url: /zh/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

表示一种编辑，在图像文档的指定区域放置彩色矩形。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | 初始化 ImageAreaRedaction 类的新实例，用于编辑特定区域大小。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getOptions()](#getOptions--) | 获取 |
RegionReplacementOptions
带有颜色和区域参数的选项。
|
|  | [getTopLeft()](#getTopLeft--) | 获取要删除区域的左上角位置 |
|
|  | [getDescription()](#getDescription--) | 返回一个字符串，描述 redaction 及其参数。 |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 将 redaction 应用于给定的格式实例。 |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


初始化 ImageAreaRedaction 类的新实例，用于编辑特定区域大小。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | topLeft | java.awt.Point | 左上区域坐标 |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | 区域大小和颜色 |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


获取
RegionReplacementOptions
带有颜色和区域参数的选项。


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


获取要删除区域的左上角位置


**Returns:**
java.awt.Point - 要删除区域的左上角位置

### getDescription() {#getDescription--}
```
public String getDescription()
```


返回一个字符串，描述 redaction 及其参数。


**Returns:**
java.lang.String - 包含 redaction 名称和参数的文本。

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


将 redaction 应用于给定的格式实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | 用于应用 redaction 的文档实例 |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

