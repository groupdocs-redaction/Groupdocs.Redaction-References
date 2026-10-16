---
title: "RedactionStatus"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示编辑完成状态。"
type: docs
weight: 20
url: /zh/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

表示编辑完成状态。

## 字段

| 字段 | 描述 |
| --- | --- |
|  | [Applied](#Applied) | 已完整且成功地应用遮蔽。 |
|
|  | [PartiallyApplied](#PartiallyApplied) | 遮蔽仅应用于其匹配项的一部分。 |
|
|  | [Skipped](#Skipped) | 遮蔽已被跳过（未应用）。 |
|
|  | [Failed](#Failed) | 遮蔽因异常而失败。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


已完整且成功地应用遮蔽。


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


遮蔽仅应用于其匹配项的一部分。


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


遮蔽已被跳过（未应用）。


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


遮蔽因异常而失败。


### values() {#values--}
```
public static RedactionStatus[] values()
```




**Returns:**
com.groupdocs.redaction.RedactionStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionStatus valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
