---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "편집 과정을 사용자 정의할 수 있는 편집 설정을 나타냅니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

Redaction 설정을 나타내며, Redaction 프로세스를 사용자 정의할 수 있습니다.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | RedactorSettings 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | 주어진 ILogger 인스턴스로 RedactorSettings 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | 주어진 IRedactionCallback 인스턴스로 RedactorSettings 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | 주어진 IOcrConnector 인스턴스로 RedactorSettings 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | 주어진 ILogger와 IRedactionCallback 인스턴스로 RedactorSettings 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | 주어진 ILogger, IRedactionCallback 및 IOcrConnector 인스턴스로 RedactorSettings 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getLogger()](#getLogger--) | 구현하는 클래스의 인스턴스를 가져옵니다 |
ILogger
, 이벤트 및 오류 로깅에 사용됩니다.
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | 구현하는 클래스의 인스턴스를 설정합니다 |
ILogger
, 이벤트 및 오류 로깅에 사용됩니다.
|
|  | [getRedactionCallback()](#getRedactionCallback--) | 구현하는 클래스의 인스턴스를 가져옵니다 |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | 구현하는 클래스의 인스턴스를 설정합니다 |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | 구현하는 클래스의 인스턴스를 가져옵니다 |
IOcrConnector
인터페이스.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | 구현하는 클래스의 인스턴스를 설정합니다 |
IOcrConnector
인터페이스.
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


RedactorSettings 클래스의 새 인스턴스를 초기화합니다.


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


주어진 ILogger 인스턴스로 RedactorSettings 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | ILogger 인터페이스를 구현하는 클래스의 인스턴스 |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


주어진 IRedactionCallback 인스턴스로 RedactorSettings 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | IRedactionCallbck 인터페이스를 구현하는 클래스의 인스턴스 |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


주어진 IOcrConnector 인스턴스로 RedactorSettings 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector 인터페이스의 유효한 구현 |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


주어진 ILogger와 IRedactionCallback 인스턴스로 RedactorSettings 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | ILogger 인터페이스를 구현하는 클래스의 인스턴스 |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | IRedactionCallbck 인터페이스를 구현하는 클래스의 인스턴스 |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


주어진 ILogger, IRedactionCallback 및 IOcrConnector 인스턴스로 RedactorSettings 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | ILogger 인터페이스를 구현하는 클래스의 인스턴스 |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | IRedactionCallbck 인터페이스를 구현하는 클래스의 인스턴스 |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector 인터페이스 구현의 인스턴스. null일 수 있습니다 |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


구현하는 클래스의 인스턴스를 가져옵니다
ILogger
, 이벤트 및 오류 로깅에 사용됩니다.


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


구현하는 클래스의 인스턴스를 설정합니다
ILogger
, 이벤트 및 오류 로깅에 사용됩니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | ILogger를 구현하는 클래스의 인스턴스로, 이벤트 및 오류 로깅에 사용됩니다. |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


구현하는 클래스의 인스턴스를 가져옵니다
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


구현하는 클래스의 인스턴스를 설정합니다
IRedactionCallback
.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | IRedactionCallback을 구현하는 클래스의 인스턴스. |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


구현하는 클래스의 인스턴스를 가져옵니다
IOcrConnector
인터페이스.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


구현하는 클래스의 인스턴스를 설정합니다
IOcrConnector
인터페이스.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector 인터페이스를 구현하는 클래스의 인스턴스. |
|

