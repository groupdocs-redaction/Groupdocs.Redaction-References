---
title: "RedactorSettings"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa la configuración de redacción que permite personalizar el proceso de redacción."
type: docs
weight: 13
url: /es/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

Representa la configuración de redacción, permitiendo personalizar el proceso de redacción.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | Inicializa una nueva instancia de la clase RedactorSettings. |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | Inicializa una nueva instancia de la clase RedactorSettings con una instancia de ILogger proporcionada. |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | Inicializa una nueva instancia de la clase RedactorSettings con una instancia de IRedactionCallback proporcionada. |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | Inicializa una nueva instancia de la clase RedactorSettings con una instancia de IOcrConnector proporcionada. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | Inicializa una nueva instancia de la clase RedactorSettings con instancias dadas de ILogger y IRedactionCallback. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | Inicializa una nueva instancia de la clase RedactorSettings con instancias dadas de ILogger, IRedactionCallback y IOcrConnector. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getLogger()](#getLogger--) | Obtiene una instancia de una clase, que implementa |
ILogger
, que se utiliza para registrar eventos y errores.
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | Establece una instancia de una clase, que implementa |
ILogger
, que se utiliza para registrar eventos y errores.
|
|  | [getRedactionCallback()](#getRedactionCallback--) | Obtiene una instancia de una clase, que implementa |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | Establece una instancia de una clase, que implementa |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | Obtiene una instancia de una clase, que implementa |
IOcrConnector
interfaz.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Establece una instancia de una clase, que implementa |
IOcrConnector
interfaz.
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


Inicializa una nueva instancia de la clase RedactorSettings.


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


Inicializa una nueva instancia de la clase RedactorSettings con una instancia de ILogger proporcionada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Una instancia de una clase que implementa la interfaz ILogger |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


Inicializa una nueva instancia de la clase RedactorSettings con una instancia de IRedactionCallback proporcionada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Una instancia de una clase que implementa la interfaz IRedactionCallbck |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


Inicializa una nueva instancia de la clase RedactorSettings con una instancia de IOcrConnector proporcionada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Una implementación válida de la interfaz IOcrConnector |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


Inicializa una nueva instancia de la clase RedactorSettings con instancias dadas de ILogger y IRedactionCallback.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Una instancia de una clase que implementa la interfaz ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Una instancia de una clase que implementa la interfaz IRedactionCallbck |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


Inicializa una nueva instancia de la clase RedactorSettings con instancias dadas de ILogger, IRedactionCallback y IOcrConnector.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Una instancia de una clase que implementa la interfaz ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Una instancia de una clase que implementa la interfaz IRedactionCallbck |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Una instancia de la implementación de la interfaz IOcrConnector. Puede ser nula |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Obtiene una instancia de una clase, que implementa
ILogger
, que se utiliza para registrar eventos y errores.


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


Establece una instancia de una clase, que implementa
ILogger
, que se utiliza para registrar eventos y errores.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Una instancia de una clase que implementa ILogger, que se utiliza para registrar eventos y errores. |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


Obtiene una instancia de una clase, que implementa
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


Establece una instancia de una clase, que implementa
IRedactionCallback
.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Una instancia de una clase que implementa IRedactionCallback. |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Obtiene una instancia de una clase, que implementa
IOcrConnector
interfaz.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Establece una instancia de una clase, que implementa
IOcrConnector
interfaz.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Una instancia de una clase que implementa la interfaz IOcrConnector. |
|

