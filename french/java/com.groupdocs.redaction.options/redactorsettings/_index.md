---
title: "RedactorSettings"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente les paramètres de rédaction permettant de personnaliser le processus de rédaction."
type: docs
weight: 13
url: /fr/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

Représente les paramètres de rédaction, permettant de personnaliser le processus de rédaction.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | Initialise une nouvelle instance de la classe RedactorSettings. |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | Initialise une nouvelle instance de la classe RedactorSettings avec une instance ILogger donnée. |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | Initialise une nouvelle instance de la classe RedactorSettings avec une instance IRedactionCallback donnée. |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | Initialise une nouvelle instance de la classe RedactorSettings avec une instance IOcrConnector donnée. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | Initialise une nouvelle instance de la classe RedactorSettings avec les instances ILogger et IRedactionCallback données. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | Initialise une nouvelle instance de la classe RedactorSettings avec les instances ILogger, IRedactionCallback et IOcrConnector données. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getLogger()](#getLogger--) | Obtient une instance d'une classe implémentant |
ILogger
, qui est utilisée pour consigner les événements et les erreurs.
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | Définit une instance d'une classe implémentant |
ILogger
, qui est utilisée pour consigner les événements et les erreurs.
|
|  | [getRedactionCallback()](#getRedactionCallback--) | Obtient une instance d'une classe implémentant |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | Définit une instance d'une classe implémentant |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | Obtient une instance d'une classe implémentant |
IOcrConnector
interface.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Définit une instance d'une classe implémentant |
IOcrConnector
interface.
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


Initialise une nouvelle instance de la classe RedactorSettings.


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


Initialise une nouvelle instance de la classe RedactorSettings avec une instance ILogger donnée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Une instance d'une classe implémentant l'interface ILogger |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


Initialise une nouvelle instance de la classe RedactorSettings avec une instance IRedactionCallback donnée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Une instance d'une classe implémentant l'interface IRedactionCallbck |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


Initialise une nouvelle instance de la classe RedactorSettings avec une instance IOcrConnector donnée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Une implémentation valide de l'interface IOcrConnector |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


Initialise une nouvelle instance de la classe RedactorSettings avec les instances ILogger et IRedactionCallback données.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Une instance d'une classe implémentant l'interface ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Une instance d'une classe implémentant l'interface IRedactionCallbck |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


Initialise une nouvelle instance de la classe RedactorSettings avec les instances ILogger, IRedactionCallback et IOcrConnector données.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Une instance d'une classe implémentant l'interface ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Une instance d'une classe implémentant l'interface IRedactionCallbck |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Une instance de l'implémentation de l'interface IOcrConnector. Peut être null |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Obtient une instance d'une classe implémentant
ILogger
, qui est utilisée pour consigner les événements et les erreurs.


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


Définit une instance d'une classe implémentant
ILogger
, qui est utilisée pour consigner les événements et les erreurs.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Une instance d'une classe implémentant ILogger, qui est utilisée pour consigner les événements et les erreurs. |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


Obtient une instance d'une classe implémentant
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


Définit une instance d'une classe implémentant
IRedactionCallback
.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Une instance d'une classe implémentant IRedactionCallback. |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Obtient une instance d'une classe implémentant
IOcrConnector
interface.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Définit une instance d'une classe implémentant
IOcrConnector
interface.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Une instance d'une classe implémentant l'interface IOcrConnector. |
|

