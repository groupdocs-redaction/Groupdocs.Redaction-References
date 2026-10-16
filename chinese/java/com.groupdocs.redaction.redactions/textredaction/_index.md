---
title: "TextRedaction"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示文档文本编辑的基础抽象类。"
type: docs
weight: 32
url: /zh/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

表示文档文本编辑的基础抽象类。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | 获取 |
ReplacementOptions
实例，指定文本替换的类型。
|
|  | [getOcrConnector()](#getOcrConnector--) | 获取 |
IOcrConnector
实现，需要从图形内容中提取文本。
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | 设置 |
IOcrConnector
实现，需要从图形内容中提取文本。
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


获取
ReplacementOptions
实例，指定文本替换的类型。


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


获取
IOcrConnector
实现，需要从图形内容中提取文本。


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


设置
IOcrConnector
实现，需要从图形内容中提取文本。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector 实现，需要从图形内容中提取文本。 |
|

