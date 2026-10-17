---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل إعدادات الحذف التي تسمح بتخصيص عملية الحذف."
type: docs
weight: 13
url: /ar/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

يمثل إعدادات التشويه، مما يسمح بتخصيص عملية التشويه.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | ينشئ مثيلًا جديدًا من فئة RedactorSettings. |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | يقوم بإنشاء نسخة جديدة من الفئة RedactorSettings باستخدام كائن ILogger معطى. |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | يقوم بإنشاء نسخة جديدة من الفئة RedactorSettings باستخدام كائن IRedactionCallback معطى. |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | يقوم بإنشاء نسخة جديدة من الفئة RedactorSettings باستخدام كائن IOcrConnector معطى. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | يقوم بإنشاء نسخة جديدة من الفئة RedactorSettings باستخدام كائنات ILogger و IRedactionCallback المعطاة. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | يقوم بإنشاء نسخة جديدة من الفئة RedactorSettings باستخدام كائنات ILogger و IRedactionCallback و IOcrConnector المعطاة. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getLogger()](#getLogger--) | يحصل على نسخة من فئة، تنفّذ |
ILogger
، التي تُستخدم لتسجيل الأحداث والأخطاء.
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | يضبط نسخة من فئة، تنفّذ |
ILogger
، التي تُستخدم لتسجيل الأحداث والأخطاء.
|
|  | [getRedactionCallback()](#getRedactionCallback--) | يحصل على نسخة من فئة، تنفّذ |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | يضبط نسخة من فئة، تنفّذ |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | يحصل على نسخة من فئة، تنفّذ |
IOcrConnector
الواجهة.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | يضبط نسخة من فئة، تنفّذ |
IOcrConnector
الواجهة.
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


ينشئ مثيلًا جديدًا من فئة RedactorSettings.


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


يقوم بإنشاء نسخة جديدة من الفئة RedactorSettings باستخدام كائن ILogger معطى.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | نسخة من فئة تنفّذ واجهة ILogger |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


يقوم بإنشاء نسخة جديدة من الفئة RedactorSettings باستخدام كائن IRedactionCallback معطى.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | نسخة من فئة تنفّذ واجهة IRedactionCallbck |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


يقوم بإنشاء نسخة جديدة من الفئة RedactorSettings باستخدام كائن IOcrConnector معطى.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | تنفيذ صالح لواجهة IOcrConnector |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


يقوم بإنشاء نسخة جديدة من الفئة RedactorSettings باستخدام كائنات ILogger و IRedactionCallback المعطاة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | نسخة من فئة تنفّذ واجهة ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | نسخة من فئة تنفّذ واجهة IRedactionCallbck |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


يقوم بإنشاء نسخة جديدة من الفئة RedactorSettings باستخدام كائنات ILogger و IRedactionCallback و IOcrConnector المعطاة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | نسخة من فئة تنفّذ واجهة ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | نسخة من فئة تنفّذ واجهة IRedactionCallbck |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | نسخة من تنفيذ واجهة IOcrConnector. يمكن أن تكون فارغة |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


يحصل على نسخة من فئة، تنفّذ
ILogger
، التي تُستخدم لتسجيل الأحداث والأخطاء.


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


يضبط نسخة من فئة، تنفّذ
ILogger
، التي تُستخدم لتسجيل الأحداث والأخطاء.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | نسخة من فئة تنفّذ  ILogger ، تُستخدم لتسجيل الأحداث والأخطاء. |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


يحصل على نسخة من فئة، تنفّذ
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


يضبط نسخة من فئة، تنفّذ
IRedactionCallback
.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | نسخة من فئة تنفّذ  IRedactionCallback . |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


يحصل على نسخة من فئة، تنفّذ
IOcrConnector
الواجهة.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


يضبط نسخة من فئة، تنفّذ
IOcrConnector
الواجهة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | نسخة من فئة تنفّذ  IOcrConnector  الواجهة. |
|

