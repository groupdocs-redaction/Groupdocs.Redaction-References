---
title: "RedactableImage"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "提供对所有光栅图像编辑操作的外观。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

提供对所有光栅图像编辑操作的外观。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | 使用实现了以下接口的对象创建新实例 |
IImageFormatInstance
接口。
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | 使用实现了以下接口的对象创建新实例 |
IMultipleAreaRedactable
接口。
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | 检索包含实际图像内容的流。 |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | 一次性使用相同颜色对多个图像区域进行编辑。 |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | 用特定颜色和尺寸的矩形替换给定点处的区域。 |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


使用实现了以下接口的对象创建新实例
IImageFormatInstance
接口。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | 实现 IImageFormatInstance 接口的实例 |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


使用实现了以下接口的对象创建新实例
IMultipleAreaRedactable
接口。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | 实现 IMultipleAreaRedactable 接口的实例 |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


检索包含实际图像内容的流。


**Returns:**
java.io.InputStream - 包含图像数据的流

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


一次性使用相同颜色对多个图像区域进行编辑。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangles | java.awt.Rectangle[] | 矩形区域的数组 |
|
|  | boxColor | java.awt.Color | 用于填充区域的颜色 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


用特定颜色和尺寸的矩形替换给定点处的区域。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | topLeft | java.awt.Point | 已填充区域左上角坐标 |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | 颜色和尺寸设置 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

