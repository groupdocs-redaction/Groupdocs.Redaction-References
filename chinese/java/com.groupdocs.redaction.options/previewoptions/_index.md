---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "提供用于设置预览生成的需求和流委托的选项。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

提供用于设置预览生成的需求和流委托的选项。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | 初始化 PreviewOptions 类的新实例，导致输出流被关闭。 |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | 初始化 PreviewOptions 类的新实例，导致输出流返回给客户端以供进一步使用。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getWidth()](#getWidth--) | 获取或设置页面预览宽度。 |
|
|  | [setWidth(int value)](#setWidth-int-) | 获取或设置页面预览宽度。 |
|
|  | [getHeight()](#getHeight--) | 获取或设置页面预览高度。 |
|
|  | [setHeight(int value)](#setHeight-int-) | 获取或设置页面预览高度。 |
|
|  | [getPageNumbers()](#getPageNumbers--) | 获取或设置用于生成预览的页面编号数组。 |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | 获取或设置用于生成预览的页面编号数组。 |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | 获取或设置预览图像格式。 |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | 获取或设置预览图像格式。 |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | 获取或设置页面流创建委托的实例。 |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | 获取或设置页面流创建委托的实例。 |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | 获取或设置页面预览完成委托的实例。 |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | 获取或设置页面预览完成委托的实例。 |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


初始化 PreviewOptions 类的新实例，导致输出流被关闭。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | 为特定页面预览创建流 |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


初始化 PreviewOptions 类的新实例，导致输出流返回给客户端以供进一步使用。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | 为特定页面预览创建流 |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | 通知页面预览生成完成并获取输出流 |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


获取或设置页面预览宽度。


**Returns:**
int - 页面预览宽度。

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


获取或设置页面预览宽度。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 页面预览宽度。 |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


获取或设置页面预览高度。


**Returns:**
int - 页面预览高度。

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


获取或设置页面预览高度。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 页面预览高度。 |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


获取或设置用于生成预览的页面编号数组。


**Returns:**
int[] - 用于生成预览的页面编号数组。

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


获取或设置用于生成预览的页面编号数组。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int[] | 用于生成预览的页面编号数组。 |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


获取或设置预览图像格式。


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


获取或设置预览图像格式。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | 预览图像格式。 |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


获取或设置页面流创建委托的实例。


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


获取或设置页面流创建委托的实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | 页面流创建委托的实例。 |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


获取或设置页面预览完成委托的实例。


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


获取或设置页面预览完成委托的实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | 页面预览完成委托的实例。 |
|

