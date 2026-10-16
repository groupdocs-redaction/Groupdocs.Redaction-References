---
title: "RedactionResult"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示编辑操作的结果。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

表示编辑操作的结果。

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getStatus()](#getStatus--) | 获取执行状态。 |
|
|  | [getErrorMessage()](#getErrorMessage--) | 获取诊断错误信息。 |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | 使用 Skipped 状态初始化 RedactionResult 类的新实例。 |
|
|  | [partial(String description)](#partial-java.lang.String-) | 使用 PartiallyApplied 状态初始化 RedactionResult 类的新实例。 |
|
|  | [failed(String description)](#failed-java.lang.String-) | 使用 Failed 状态初始化 RedactionResult 类的新实例。 |
|
|  | [successful()](#successful--) | 使用 Applied（成功）状态初始化 RedactionResult 类的新实例。 |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


获取执行状态。


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


获取诊断错误信息。


**Returns:**
java.lang.String - 诊断错误信息。

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


使用 Skipped 状态初始化 RedactionResult 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 描述 | java.lang.String | 操作被跳过的原因 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


使用 PartiallyApplied 状态初始化 RedactionResult 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 描述 | java.lang.String | 操作未完全应用的原因 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


使用 Failed 状态初始化 RedactionResult 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 描述 | java.lang.String | 失败或异常详细信息 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


使用 Applied（成功）状态初始化 RedactionResult 类的新实例。


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

