---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει τις ρυθμίσεις διαγραφής που επιτρέπουν την προσαρμογή της διαδικασίας διαγραφής."
type: docs
weight: 13
url: /el/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

Αντιπροσωπεύει τις ρυθμίσεις επεξεργασίας, επιτρέποντας την προσαρμογή της διαδικασίας επεξεργασίας.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης RedactorSettings. |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | Αρχικοποιεί μια νέα παρουσία της κλάσης RedactorSettings με ένα δεδομένο αντικείμενο ILogger. |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | Αρχικοποιεί μια νέα παρουσία της κλάσης RedactorSettings με ένα δεδομένο αντικείμενο IRedactionCallback. |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | Αρχικοποιεί μια νέα παρουσία της κλάσης RedactorSettings με ένα δεδομένο αντικείμενο IOcrConnector. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | Αρχικοποιεί μια νέα παρουσία της κλάσης RedactorSettings με δεδομένα αντικείμενα ILogger και IRedactionCallback. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | Αρχικοποιεί μια νέα παρουσία της κλάσης RedactorSettings με δεδομένα αντικείμενα ILogger, IRedactionCallback και IOcrConnector. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getLogger()](#getLogger--) | Λαμβάνει μια παρουσία μιας κλάσης, η οποία υλοποιεί |
ILogger
, η οποία χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων.
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | Ορίζει μια παρουσία μιας κλάσης, η οποία υλοποιεί |
ILogger
, η οποία χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων.
|
|  | [getRedactionCallback()](#getRedactionCallback--) | Λαμβάνει μια παρουσία μιας κλάσης, η οποία υλοποιεί |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | Ορίζει μια παρουσία μιας κλάσης, η οποία υλοποιεί |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | Λαμβάνει μια παρουσία μιας κλάσης, η οποία υλοποιεί |
IOcrConnector
διασύνδεση.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Ορίζει μια παρουσία μιας κλάσης, η οποία υλοποιεί |
IOcrConnector
διασύνδεση.
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης RedactorSettings.


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης RedactorSettings με ένα δεδομένο αντικείμενο ILogger.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Μια παρουσία μιας κλάσης, η οποία υλοποιεί τη διασύνδεση ILogger |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης RedactorSettings με ένα δεδομένο αντικείμενο IRedactionCallback.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Μια παρουσία μιας κλάσης, η οποία υλοποιεί τη διασύνδεση IRedactionCallbck |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης RedactorSettings με ένα δεδομένο αντικείμενο IOcrConnector.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Μια έγκυρη υλοποίηση της διασύνδεσης IOcrConnector |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης RedactorSettings με δεδομένα αντικείμενα ILogger και IRedactionCallback.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Μια παρουσία μιας κλάσης, η οποία υλοποιεί τη διασύνδεση ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Μια παρουσία μιας κλάσης, η οποία υλοποιεί τη διασύνδεση IRedactionCallbck |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης RedactorSettings με δεδομένα αντικείμενα ILogger, IRedactionCallback και IOcrConnector.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Μια παρουσία μιας κλάσης, η οποία υλοποιεί τη διασύνδεση ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Μια παρουσία μιας κλάσης, η οποία υλοποιεί τη διασύνδεση IRedactionCallbck |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Μια παρουσία υλοποίησης της διασύνδεσης IOcrConnector. Μπορεί να είναι null |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Λαμβάνει μια παρουσία μιας κλάσης, η οποία υλοποιεί
ILogger
, η οποία χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων.


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


Ορίζει μια παρουσία μιας κλάσης, η οποία υλοποιεί
ILogger
, η οποία χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Μια παρουσία μιας κλάσης, η οποία υλοποιεί το ILogger, και χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων. |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


Λαμβάνει μια παρουσία μιας κλάσης, η οποία υλοποιεί
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


Ορίζει μια παρουσία μιας κλάσης, η οποία υλοποιεί
IRedactionCallback
.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Μια παρουσία μιας κλάσης, η οποία υλοποιεί το IRedactionCallback. |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Λαμβάνει μια παρουσία μιας κλάσης, η οποία υλοποιεί
IOcrConnector
διασύνδεση.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Ορίζει μια παρουσία μιας κλάσης, η οποία υλοποιεί
IOcrConnector
διασύνδεση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Μια παρουσία μιας κλάσης, η οποία υλοποιεί τη διασύνδεση IOcrConnector. |
|

