---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Kırpma ayarlarını temsil eder ve kırpma sürecini özelleştirmeye izin verir."
type: docs
weight: 13
url: /tr/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

Kırpma ayarlarını temsil eder, kırpma sürecini özelleştirmeye izin verir.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | RedactorSettings sınıfının yeni bir örneğini başlatır. |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | RedactorSettings sınıfının yeni bir örneğini verilen ILogger örneğiyle başlatır. |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | RedactorSettings sınıfının yeni bir örneğini verilen IRedactionCallback örneğiyle başlatır. |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | RedactorSettings sınıfının yeni bir örneğini verilen IOcrConnector örneğiyle başlatır. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | RedactorSettings sınıfının yeni bir örneğini verilen ILogger ve IRedactionCallback örnekleriyle başlatır. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | RedactorSettings sınıfının yeni bir örneğini verilen ILogger, IRedactionCallback ve IOcrConnector örnekleriyle başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getLogger()](#getLogger--) | Uygulayan bir sınıfın örneğini alır |
ILogger
, olayları ve hataları kaydetmek için kullanılır.
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | Uygulayan bir sınıfın örneğini ayarlar |
ILogger
, olayları ve hataları kaydetmek için kullanılır.
|
|  | [getRedactionCallback()](#getRedactionCallback--) | Uygulayan bir sınıfın örneğini alır |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | Uygulayan bir sınıfın örneğini ayarlar |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | Uygulayan bir sınıfın örneğini alır |
IOcrConnector
arayüz.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Uygulayan bir sınıfın örneğini ayarlar |
IOcrConnector
arayüz.
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


RedactorSettings sınıfının yeni bir örneğini başlatır.


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


RedactorSettings sınıfının yeni bir örneğini verilen ILogger örneğiyle başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | ILogger arayüzünü uygulayan bir sınıfın örneği |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


RedactorSettings sınıfının yeni bir örneğini verilen IRedactionCallback örneğiyle başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | IRedactionCallbck arayüzünü uygulayan bir sınıfın örneği |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


RedactorSettings sınıfının yeni bir örneğini verilen IOcrConnector örneğiyle başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector arayüzünün geçerli bir uygulaması |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


RedactorSettings sınıfının yeni bir örneğini verilen ILogger ve IRedactionCallback örnekleriyle başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | ILogger arayüzünü uygulayan bir sınıfın örneği |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | IRedactionCallbck arayüzünü uygulayan bir sınıfın örneği |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


RedactorSettings sınıfının yeni bir örneğini verilen ILogger, IRedactionCallback ve IOcrConnector örnekleriyle başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | ILogger arayüzünü uygulayan bir sınıfın örneği |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | IRedactionCallbck arayüzünü uygulayan bir sınıfın örneği |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector arabirimi uygulamasının bir örneği. Null olabilir |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Uygulayan bir sınıfın örneğini alır
ILogger
, olayları ve hataları kaydetmek için kullanılır.


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


Uygulayan bir sınıfın örneğini ayarlar
ILogger
, olayları ve hataları kaydetmek için kullanılır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Olayları ve hataları kaydetmek için kullanılan, ILogger uygulayan bir sınıfın örneği. |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


Uygulayan bir sınıfın örneğini alır
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


Uygulayan bir sınıfın örneğini ayarlar
IRedactionCallback
.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | IRedactionCallback uygulayan bir sınıfın örneği. |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Uygulayan bir sınıfın örneğini alır
IOcrConnector
arayüz.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Uygulayan bir sınıfın örneğini ayarlar
IOcrConnector
arayüz.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector arabirimini uygulayan bir sınıfın örneği. |
|

