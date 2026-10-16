---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta le impostazioni di redazione che consentono di personalizzare il processo di redazione."
type: docs
weight: 13
url: /it/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

Rappresenta le impostazioni di redazione, consentendo di personalizzare il processo di redazione.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | Inizializza una nuova istanza della classe RedactorSettings. |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | Inizializza una nuova istanza della classe RedactorSettings con una determinata istanza di ILogger. |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | Inizializza una nuova istanza della classe RedactorSettings con una determinata istanza di IRedactionCallback. |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | Inizializza una nuova istanza della classe RedactorSettings con una determinata istanza di IOcrConnector. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | Inizializza una nuova istanza della classe RedactorSettings con le istanze fornite di ILogger e IRedactionCallback. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | Inizializza una nuova istanza della classe RedactorSettings con le istanze fornite di ILogger, IRedactionCallback e IOcrConnector. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getLogger()](#getLogger--) | Ottiene un'istanza di una classe, che implementa |
ILogger
, che è usata per registrare eventi ed errori.
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | Imposta un'istanza di una classe, che implementa |
ILogger
, che è usata per registrare eventi ed errori.
|
|  | [getRedactionCallback()](#getRedactionCallback--) | Ottiene un'istanza di una classe, che implementa |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | Imposta un'istanza di una classe, che implementa |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | Ottiene un'istanza di una classe, che implementa |
IOcrConnector
interfaccia.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Imposta un'istanza di una classe, che implementa |
IOcrConnector
interfaccia.
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


Inizializza una nuova istanza della classe RedactorSettings.


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


Inizializza una nuova istanza della classe RedactorSettings con una determinata istanza di ILogger.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Un'istanza di una classe, che implementa l'interfaccia ILogger |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


Inizializza una nuova istanza della classe RedactorSettings con una determinata istanza di IRedactionCallback.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Un'istanza di una classe, che implementa l'interfaccia IRedactionCallbck |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


Inizializza una nuova istanza della classe RedactorSettings con una determinata istanza di IOcrConnector.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Una valida implementazione dell'interfaccia IOcrConnector |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


Inizializza una nuova istanza della classe RedactorSettings con le istanze fornite di ILogger e IRedactionCallback.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Un'istanza di una classe, che implementa l'interfaccia ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Un'istanza di una classe, che implementa l'interfaccia IRedactionCallbck |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


Inizializza una nuova istanza della classe RedactorSettings con le istanze fornite di ILogger, IRedactionCallback e IOcrConnector.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Un'istanza di una classe, che implementa l'interfaccia ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Un'istanza di una classe, che implementa l'interfaccia IRedactionCallbck |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Un'istanza dell'implementazione dell'interfaccia IOcrConnector. Può essere null |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Ottiene un'istanza di una classe, che implementa
ILogger
, che è usata per registrare eventi ed errori.


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


Imposta un'istanza di una classe, che implementa
ILogger
, che è usata per registrare eventi ed errori.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Un'istanza di una classe, che implementa ILogger, che è usata per registrare eventi ed errori. |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


Ottiene un'istanza di una classe, che implementa
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


Imposta un'istanza di una classe, che implementa
IRedactionCallback
.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Un'istanza di una classe, che implementa IRedactionCallback. |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Ottiene un'istanza di una classe, che implementa
IOcrConnector
interfaccia.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Imposta un'istanza di una classe, che implementa
IOcrConnector
interfaccia.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Un'istanza di una classe, che implementa l'interfaccia IOcrConnector. |
|

