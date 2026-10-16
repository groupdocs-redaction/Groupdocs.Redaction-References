---
title: "编辑"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示所有编辑类型的基础抽象类。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

表示所有编辑类型的基础抽象类。

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getDescription()](#getDescription--) | 返回一个字符串，描述 redaction 及其参数。 |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 将 redaction 应用于给定的格式实例。 |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


返回一个字符串，描述 redaction 及其参数。


**Returns:**
java.lang.String - 包含 redaction 名称和参数的文本。

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


将 redaction 应用于给定的格式实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | 用于应用 redaction 的文档实例 |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

