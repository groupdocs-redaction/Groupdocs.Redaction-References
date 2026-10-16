---
title: "ReplacementType"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示匹配文本的替换类型。"
type: docs
weight: 38
url: /zh/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

表示匹配文本的替换类型。

## 字段

| 字段 | 描述 |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | 将匹配的文本替换为另一个字符串，例如。 |
|
|  | [DrawBox](#DrawBox) | 绘制特定颜色的矩形（默认黑色）以替代已编辑的文本。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


将匹配的文本替换为另一个字符串，例如豁免代码。


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


绘制特定颜色的矩形（默认黑色）以替代已编辑的文本。


### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
