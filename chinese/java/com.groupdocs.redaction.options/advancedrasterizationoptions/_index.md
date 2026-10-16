---
title: "AdvancedRasterizationOptions"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "用于管理要应用的高级光栅化选项的枚举。"
type: docs
weight: 19
url: /zh/java/com.groupdocs.redaction.options/advancedrasterizationoptions/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum AdvancedRasterizationOptions extends Enum<AdvancedRasterizationOptions>
```

用于管理要应用的高级光栅化选项的枚举。

## 字段

| 字段 | 描述 |
| --- | --- |
|  | [Tilt](#Tilt) | 倾斜光栅化图像，使其以随机角度倾斜。 |
|
|  | [Noise](#Noise) | 在光栅化的页面图像上添加随机斑点。 |
|
|  | [Border](#Border) | 添加边框线以模拟页面扫描效果。 |
|
|  | [Grayscale](#Grayscale) | 将页面图像转换为灰度，以模拟灰度扫描。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Tilt {#Tilt}
```
public static final AdvancedRasterizationOptions Tilt
```


倾斜光栅化图像，使其以随机角度倾斜。


### Noise {#Noise}
```
public static final AdvancedRasterizationOptions Noise
```


在光栅化的页面图像上添加随机斑点。


### Border {#Border}
```
public static final AdvancedRasterizationOptions Border
```


添加边框线以模拟页面扫描效果。


### Grayscale {#Grayscale}
```
public static final AdvancedRasterizationOptions Grayscale
```


将页面图像转换为灰度，以模拟灰度扫描。


### values() {#values--}
```
public static AdvancedRasterizationOptions[] values()
```




**Returns:**
com.groupdocs.redaction.options.AdvancedRasterizationOptions[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static AdvancedRasterizationOptions valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions)
