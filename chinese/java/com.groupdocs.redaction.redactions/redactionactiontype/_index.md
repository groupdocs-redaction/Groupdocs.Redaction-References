---
title: "RedactionActionType"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示可用于执行编辑的操作。"
type: docs
weight: 37
url: /zh/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

表示可用于执行编辑的操作。

## 字段

| 字段 | 描述 |
| --- | --- |
|  | [Replacement](#Replacement) | 已编辑的文本被替换为其他文本或被块覆盖。 |
|
|  | [Cleanup](#Cleanup) | 数据已被删除，但文档中仍保留一个空对象。 |
|
|  | [Deletion](#Deletion) | 文档中的数据及相关结构已被删除。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


已编辑的文本被替换为其他文本或被块覆盖。


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


数据已被删除，但文档中仍保留一个空对象。


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


文档中的数据及相关结构已被删除。


### values() {#values--}
```
public static RedactionActionType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.RedactionActionType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionActionType valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
