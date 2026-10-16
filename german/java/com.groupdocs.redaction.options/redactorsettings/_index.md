---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Redaktions-Einstellungen dar, die die Anpassung des Redaktionsprozesses ermöglichen."
type: docs
weight: 13
url: /de/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

Stellt Redaktions‑Einstellungen dar, die es ermöglichen, den Redaktionsprozess anzupassen.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | Initialisiert eine neue Instanz der Klasse RedactorSettings. |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | Initialisiert eine neue Instanz der Klasse RedactorSettings mit einer angegebenen ILogger-Instanz. |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | Initialisiert eine neue Instanz der Klasse RedactorSettings mit einer angegebenen IRedactionCallback-Instanz. |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | Initialisiert eine neue Instanz der Klasse RedactorSettings mit einer angegebenen IOcrConnector-Instanz. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | Initialisiert eine neue Instanz der Klasse RedactorSettings mit angegebenen ILogger- und IRedactionCallback-Instanzen. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | Initialisiert eine neue Instanz der Klasse RedactorSettings mit angegebenen ILogger-, IRedactionCallback- und IOcrConnector-Instanzen. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getLogger()](#getLogger--) | Erhält eine Instanz einer Klasse, die implementiert |
ILogger
, die für das Protokollieren von Ereignissen und Fehlern verwendet wird.
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | Setzt eine Instanz einer Klasse, die implementiert |
ILogger
, die für das Protokollieren von Ereignissen und Fehlern verwendet wird.
|
|  | [getRedactionCallback()](#getRedactionCallback--) | Erhält eine Instanz einer Klasse, die implementiert |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | Setzt eine Instanz einer Klasse, die implementiert |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | Erhält eine Instanz einer Klasse, die implementiert |
IOcrConnector
Schnittstelle.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Setzt eine Instanz einer Klasse, die implementiert |
IOcrConnector
Schnittstelle.
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


Initialisiert eine neue Instanz der Klasse RedactorSettings.


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


Initialisiert eine neue Instanz der Klasse RedactorSettings mit einer angegebenen ILogger-Instanz.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Eine Instanz einer Klasse, die die ILogger-Schnittstelle implementiert |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


Initialisiert eine neue Instanz der Klasse RedactorSettings mit einer angegebenen IRedactionCallback-Instanz.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Eine Instanz einer Klasse, die die IRedactionCallbck-Schnittstelle implementiert |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


Initialisiert eine neue Instanz der Klasse RedactorSettings mit einer angegebenen IOcrConnector-Instanz.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Eine gültige Implementierung der IOcrConnector-Schnittstelle |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


Initialisiert eine neue Instanz der Klasse RedactorSettings mit angegebenen ILogger- und IRedactionCallback-Instanzen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Eine Instanz einer Klasse, die die ILogger-Schnittstelle implementiert |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Eine Instanz einer Klasse, die die IRedactionCallbck-Schnittstelle implementiert |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


Initialisiert eine neue Instanz der Klasse RedactorSettings mit angegebenen ILogger-, IRedactionCallback- und IOcrConnector-Instanzen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Eine Instanz einer Klasse, die die ILogger-Schnittstelle implementiert |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Eine Instanz einer Klasse, die die IRedactionCallbck-Schnittstelle implementiert |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Eine Instanz der IOcrConnector Schnittstellenimplementierung. Kann null sein |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Erhält eine Instanz einer Klasse, die implementiert
ILogger
, die für das Protokollieren von Ereignissen und Fehlern verwendet wird.


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


Setzt eine Instanz einer Klasse, die implementiert
ILogger
, die für das Protokollieren von Ereignissen und Fehlern verwendet wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Eine Instanz einer Klasse, die ILogger implementiert und für das Protokollieren von Ereignissen und Fehlern verwendet wird. |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


Erhält eine Instanz einer Klasse, die implementiert
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


Setzt eine Instanz einer Klasse, die implementiert
IRedactionCallback
.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Eine Instanz einer Klasse, die IRedactionCallback implementiert. |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Erhält eine Instanz einer Klasse, die implementiert
IOcrConnector
Schnittstelle.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Setzt eine Instanz einer Klasse, die implementiert
IOcrConnector
Schnittstelle.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Eine Instanz einer Klasse, die die IOcrConnector Schnittstelle implementiert. |
|

