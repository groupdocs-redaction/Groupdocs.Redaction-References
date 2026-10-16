---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示允许自定义脱敏过程的脱敏设置。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

表示编辑设置，允许自定义编辑过程。

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | 初始化 RedactorSettings 类的新实例。 |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | 初始化 RedactorSettings 类的新实例，使用给定的 ILogger 实例。 |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | 初始化 RedactorSettings 类的新实例，使用给定的 IRedactionCallback 实例。 |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | 初始化 RedactorSettings 类的新实例，使用给定的 IOcrConnector 实例。 |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | 初始化 RedactorSettings 类的新实例，使用给定的 ILogger 和 IRedactionCallback 实例。 |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | 初始化 RedactorSettings 类的新实例，使用给定的 ILogger、IRedactionCallback 和 IOcrConnector 实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getLogger()](#getLogger--) | 获取实现了 |
ILogger
，用于记录事件和错误。
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | 设置实现了 |
ILogger
，用于记录事件和错误。
|
|  | [getRedactionCallback()](#getRedactionCallback--) | 获取实现了 |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | 设置实现了 |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | 获取实现了 |
IOcrConnector
接口。
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | 设置实现了 |
IOcrConnector
接口。
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


初始化 RedactorSettings 类的新实例。


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


初始化 RedactorSettings 类的新实例，使用给定的 ILogger 实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | 实现 ILogger 接口的类的实例 |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


初始化 RedactorSettings 类的新实例，使用给定的 IRedactionCallback 实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | 实现 IRedactionCallbck 接口的类的实例 |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


初始化 RedactorSettings 类的新实例，使用给定的 IOcrConnector 实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector 接口的有效实现 |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


初始化 RedactorSettings 类的新实例，使用给定的 ILogger 和 IRedactionCallback 实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | 实现 ILogger 接口的类的实例 |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | 实现 IRedactionCallbck 接口的类的实例 |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


初始化 RedactorSettings 类的新实例，使用给定的 ILogger、IRedactionCallback 和 IOcrConnector 实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | 实现 ILogger 接口的类的实例 |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | 实现 IRedactionCallbck 接口的类的实例 |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector 接口实现的实例。可以为 null |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


获取实现了
ILogger
，用于记录事件和错误。


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


设置实现了
ILogger
，用于记录事件和错误。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | 实现了 ILogger 的类的实例，用于记录事件和错误。 |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


获取实现了
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


设置实现了
IRedactionCallback
.


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | 实现了 IRedactionCallback 的类的实例。 |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


获取实现了
IOcrConnector
接口。


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


设置实现了
IOcrConnector
接口。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | 实现了 IOcrConnector 接口的类的实例。 |
|

