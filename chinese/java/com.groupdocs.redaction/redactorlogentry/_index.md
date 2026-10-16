---
title: "RedactorLogEntry"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示应用编辑的结果。"
type: docs
weight: 18
url: /zh/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

表示应用编辑的结果。

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | 为编辑初始化 RedactorLogEntry 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getResult()](#getResult--) | 获取由...返回的结果， |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | 获取对编辑及其选项的引用。 |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


为编辑初始化 RedactorLogEntry 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | 对编辑的引用 |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | 编辑结果，由格式处理程序报告 |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


获取由...返回的结果，
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


获取对编辑及其选项的引用。


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

