---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示文档元数据编辑的基础抽象类。"
type: docs
weight: 20
url: /zh/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

表示文档元数据编辑的基础抽象类。

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFilter()](#getFilter--) | 获取用于选择全部或特定元数据（例如 Author 或 Company）的过滤器。 |
|
|  | [setFilter(int value)](#setFilter-int-) | 设置用于选择全部或特定元数据（例如 Author 或 Company）的过滤器。 |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 将 redaction 应用于给定的格式实例。 |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


获取用于选择全部或特定元数据（例如 Author 或 Company）的过滤器。


**Returns:**
int - 用于选择全部或特定元数据（例如 Author 或 Company）的过滤器。

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


设置用于选择全部或特定元数据（例如 Author 或 Company）的过滤器。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 用于选择全部或特定元数据（例如 Author 或 Company）的过滤器。 |
|

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

