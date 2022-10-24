---
title: RedactorSettings
second_title: GroupDocs.Redaction for Java API Reference
description: Represents redaction settings allowing to customize the redaction process.
type: docs
weight: 13
url: /java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

Represents redaction settings, allowing to customize the redaction process.

--------------------

**Learn more**

 *  More details about implementing ILogger interface: [Use advanced logging][]
 *  More details about implementing IRedactionCallback interface: [Use redaction callback][]


[Use advanced logging]: https://docs.groupdocs.com/redaction/java/use-advanced-logging/
[Use redaction callback]: https://docs.groupdocs.com/redaction/java/use-redaction-callback/
## Constructors

| Constructor | Description |
| --- | --- |
| [RedactorSettings()](#RedactorSettings--) | Initializes a new instance of the RedactorSettings class. |
| [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | Initializes a new instance of the RedactorSettings class with a given ILogger instance. |
| [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | Initializes a new instance of the RedactorSettings class with a given IRedactionCallback instance. |
| [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | Initializes a new instance of the RedactorSettings class with a given IOcrConnector instance. |
| [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | Initializes a new instance of the RedactorSettings class with given ILogger and IRedactionCallback instances. |
| [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | Initializes a new instance of the RedactorSettings class with given ILogger, IRedactionCallback and IOcrConnector instances. |
## Methods

| Method | Description |
| --- | --- |
| [getLogger()](#getLogger--) | Gets an instance of a class, implementing  ILogger , that is used for logging events and errors. |
| [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | Sets an instance of a class, implementing  ILogger , that is used for logging events and errors. |
| [getRedactionCallback()](#getRedactionCallback--) | Gets an instance of a class, implementing  IRedactionCallback . |
| [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | Sets an instance of a class, implementing  IRedactionCallback . |
| [getOcrConnector()](#getOcrConnector--) | Gets an instance of a class, implementing  IOcrConnector  interface. |
| [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Sets an instance of a class, implementing  IOcrConnector  interface. |
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


Initializes a new instance of the RedactorSettings class.

### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


Initializes a new instance of the RedactorSettings class with a given ILogger instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | An instance of a class, implementing ILogger interface |

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


Initializes a new instance of the RedactorSettings class with a given IRedactionCallback instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | An instance of a class, implementing IRedactionCallbck interface |

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


Initializes a new instance of the RedactorSettings class with a given IOcrConnector instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | A valid implementation of IOcrConnector interface |

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


Initializes a new instance of the RedactorSettings class with given ILogger and IRedactionCallback instances.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | An instance of a class, implementing ILogger interface |
| callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | An instance of a class, implementing IRedactionCallbck interface |

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


Initializes a new instance of the RedactorSettings class with given ILogger, IRedactionCallback and IOcrConnector instances.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | An instance of a class, implementing ILogger interface |
| callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | An instance of a class, implementing IRedactionCallbck interface |
| ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | An instance of IOcrConnector interface implementation. Can be null |

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Gets an instance of a class, implementing  ILogger , that is used for logging events and errors.

**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.
### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


Sets an instance of a class, implementing  ILogger , that is used for logging events and errors.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | An instance of a class, implementing  ILogger , that is used for logging events and errors. |

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


Gets an instance of a class, implementing  IRedactionCallback .

**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .
### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


Sets an instance of a class, implementing  IRedactionCallback .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | An instance of a class, implementing  IRedactionCallback . |

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Gets an instance of a class, implementing  IOcrConnector  interface.

**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.
### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Sets an instance of a class, implementing  IOcrConnector  interface.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | An instance of a class, implementing  IOcrConnector  interface. |

