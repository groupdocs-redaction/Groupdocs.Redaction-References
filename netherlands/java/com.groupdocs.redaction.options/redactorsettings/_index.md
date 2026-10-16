---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt redactie-instellingen voor die het aanpassen van het redactieproces mogelijk maken."
type: docs
weight: 13
url: /nl/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

Stelt redactiesettings voor, waarmee het redactieproces kan worden aangepast.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse. |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met een opgegeven ILogger-instantie. |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met een opgegeven IRedactionCallback-instantie. |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met een opgegeven IOcrConnector-instantie. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met gegeven ILogger- en IRedactionCallback-instanties. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met gegeven ILogger-, IRedactionCallback- en IOcrConnector-instanties. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getLogger()](#getLogger--) | Haalt een exemplaar van een klasse op, die implementeert |
ILogger
, die wordt gebruikt voor het loggen van gebeurtenissen en fouten.
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | Stelt een exemplaar van een klasse in, die implementeert |
ILogger
, die wordt gebruikt voor het loggen van gebeurtenissen en fouten.
|
|  | [getRedactionCallback()](#getRedactionCallback--) | Haalt een exemplaar van een klasse op, die implementeert |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | Stelt een exemplaar van een klasse in, die implementeert |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | Haalt een exemplaar van een klasse op, die implementeert |
IOcrConnector
interface.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Stelt een exemplaar van een klasse in, die implementeert |
IOcrConnector
interface.
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


Initialiseert een nieuw exemplaar van de RedactorSettings-klasse.


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met een opgegeven ILogger-instantie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Een exemplaar van een klasse, die de ILogger-interface implementeert |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met een opgegeven IRedactionCallback-instantie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Een exemplaar van een klasse, die de IRedactionCallbck-interface implementeert |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met een opgegeven IOcrConnector-instantie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Een geldige implementatie van de IOcrConnector-interface |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met gegeven ILogger- en IRedactionCallback-instanties.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Een exemplaar van een klasse, die de ILogger-interface implementeert |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Een exemplaar van een klasse, die de IRedactionCallbck-interface implementeert |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met gegeven ILogger-, IRedactionCallback- en IOcrConnector-instanties.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Een exemplaar van een klasse, die de ILogger-interface implementeert |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Een exemplaar van een klasse, die de IRedactionCallbck-interface implementeert |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Een exemplaar van een IOcrConnector-interface-implementatie. Kan null zijn |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Haalt een exemplaar van een klasse op, die implementeert
ILogger
, die wordt gebruikt voor het loggen van gebeurtenissen en fouten.


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


Stelt een exemplaar van een klasse in, die implementeert
ILogger
, die wordt gebruikt voor het loggen van gebeurtenissen en fouten.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Een exemplaar van een klasse, die  ILogger  implementeert, die wordt gebruikt voor het loggen van gebeurtenissen en fouten. |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


Haalt een exemplaar van een klasse op, die implementeert
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


Stelt een exemplaar van een klasse in, die implementeert
IRedactionCallback
.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Een exemplaar van een klasse, die  IRedactionCallback  implementeert. |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Haalt een exemplaar van een klasse op, die implementeert
IOcrConnector
interface.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Stelt een exemplaar van een klasse in, die implementeert
IOcrConnector
interface.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Een exemplaar van een klasse, die  IOcrConnector  interface implementeert. |
|

