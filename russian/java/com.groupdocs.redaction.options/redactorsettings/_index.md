---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет настройки редактирования, позволяющие настроить процесс редактирования."
type: docs
weight: 13
url: /ru/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

Представляет настройки редактирования, позволяющие настраивать процесс редактирования.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | Инициализирует новый экземпляр класса RedactorSettings. |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | Инициализирует новый экземпляр класса RedactorSettings с заданным экземпляром ILogger. |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | Инициализирует новый экземпляр класса RedactorSettings с заданным экземпляром IRedactionCallback. |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | Инициализирует новый экземпляр класса RedactorSettings с заданным экземпляром IOcrConnector. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | Инициализирует новый экземпляр класса RedactorSettings с заданными экземплярами ILogger и IRedactionCallback. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | Инициализирует новый экземпляр класса RedactorSettings с заданными экземплярами ILogger, IRedactionCallback и IOcrConnector. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getLogger()](#getLogger--) | Получает экземпляр класса, реализующего |
ILogger
, который используется для журналирования событий и ошибок.
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | Устанавливает экземпляр класса, реализующего |
ILogger
, который используется для журналирования событий и ошибок.
|
|  | [getRedactionCallback()](#getRedactionCallback--) | Получает экземпляр класса, реализующего |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | Устанавливает экземпляр класса, реализующего |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | Получает экземпляр класса, реализующего |
IOcrConnector
интерфейс.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Устанавливает экземпляр класса, реализующего |
IOcrConnector
интерфейс.
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


Инициализирует новый экземпляр класса RedactorSettings.


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


Инициализирует новый экземпляр класса RedactorSettings с заданным экземпляром ILogger.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Экземпляр класса, реализующего интерфейс ILogger |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


Инициализирует новый экземпляр класса RedactorSettings с заданным экземпляром IRedactionCallback.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Экземпляр класса, реализующего интерфейс IRedactionCallbck |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


Инициализирует новый экземпляр класса RedactorSettings с заданным экземпляром IOcrConnector.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Корректная реализация интерфейса IOcrConnector |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


Инициализирует новый экземпляр класса RedactorSettings с заданными экземплярами ILogger и IRedactionCallback.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Экземпляр класса, реализующего интерфейс ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Экземпляр класса, реализующего интерфейс IRedactionCallbck |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


Инициализирует новый экземпляр класса RedactorSettings с заданными экземплярами ILogger, IRedactionCallback и IOcrConnector.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Экземпляр класса, реализующего интерфейс ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Экземпляр класса, реализующего интерфейс IRedactionCallbck |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Экземпляр реализации интерфейса IOcrConnector. Может быть null |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Получает экземпляр класса, реализующего
ILogger
, который используется для журналирования событий и ошибок.


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


Устанавливает экземпляр класса, реализующего
ILogger
, который используется для журналирования событий и ошибок.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Экземпляр класса, реализующего ILogger, который используется для журналирования событий и ошибок. |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


Получает экземпляр класса, реализующего
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


Устанавливает экземпляр класса, реализующего
IRedactionCallback
.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Экземпляр класса, реализующего IRedactionCallback. |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Получает экземпляр класса, реализующего
IOcrConnector
интерфейс.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Устанавливает экземпляр класса, реализующего
IOcrConnector
интерфейс.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Экземпляр класса, реализующего интерфейс IOcrConnector. |
|

