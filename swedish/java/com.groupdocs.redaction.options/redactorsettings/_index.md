---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar raderingsinställningar som möjliggör anpassning av raderingsprocessen."
type: docs
weight: 13
url: /sv/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

Representerar raderingsinställningar som möjliggör anpassning av raderingsprocessen.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | Initierar en ny instans av klassen RedactorSettings. |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | Initierar en ny instans av klassen RedactorSettings med en given ILogger-instans. |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | Initierar en ny instans av klassen RedactorSettings med en given IRedactionCallback-instans. |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | Initierar en ny instans av klassen RedactorSettings med en given IOcrConnector-instans. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | Initierar en ny instans av klassen RedactorSettings med givna ILogger- och IRedactionCallback-instanser. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | Initierar en ny instans av klassen RedactorSettings med givna ILogger-, IRedactionCallback- och IOcrConnector-instanser. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getLogger()](#getLogger--) | Hämtar en instans av en klass, som implementerar |
ILogger
, som används för att logga händelser och fel.
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | Ställer in en instans av en klass, som implementerar |
ILogger
, som används för att logga händelser och fel.
|
|  | [getRedactionCallback()](#getRedactionCallback--) | Hämtar en instans av en klass, som implementerar |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | Ställer in en instans av en klass, som implementerar |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | Hämtar en instans av en klass, som implementerar |
IOcrConnector
gränssnitt.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Ställer in en instans av en klass, som implementerar |
IOcrConnector
gränssnitt.
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


Initierar en ny instans av klassen RedactorSettings.


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


Initierar en ny instans av klassen RedactorSettings med en given ILogger-instans.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | En instans av en klass som implementerar ILogger-gränssnittet |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


Initierar en ny instans av klassen RedactorSettings med en given IRedactionCallback-instans.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | En instans av en klass som implementerar IRedactionCallbck-gränssnittet |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


Initierar en ny instans av klassen RedactorSettings med en given IOcrConnector-instans.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | En giltig implementation av IOcrConnector-gränssnittet |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


Initierar en ny instans av klassen RedactorSettings med givna ILogger- och IRedactionCallback-instanser.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | En instans av en klass som implementerar ILogger-gränssnittet |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | En instans av en klass som implementerar IRedactionCallbck-gränssnittet |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


Initierar en ny instans av klassen RedactorSettings med givna ILogger-, IRedactionCallback- och IOcrConnector-instanser.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | En instans av en klass som implementerar ILogger-gränssnittet |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | En instans av en klass som implementerar IRedactionCallbck-gränssnittet |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | En instans av IOcrConnector-gränssnittimplementation. Kan vara null |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Hämtar en instans av en klass, som implementerar
ILogger
, som används för att logga händelser och fel.


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


Ställer in en instans av en klass, som implementerar
ILogger
, som används för att logga händelser och fel.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | En instans av en klass som implementerar  ILogger , som används för att logga händelser och fel. |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


Hämtar en instans av en klass, som implementerar
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


Ställer in en instans av en klass, som implementerar
IRedactionCallback
.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | En instans av en klass som implementerar  IRedactionCallback . |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Hämtar en instans av en klass, som implementerar
IOcrConnector
gränssnitt.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Ställer in en instans av en klass, som implementerar
IOcrConnector
gränssnitt.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | En instans av en klass som implementerar  IOcrConnector  gränssnitt. |
|

