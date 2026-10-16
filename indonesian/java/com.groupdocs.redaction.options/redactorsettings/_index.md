---
title: "RedactorSettings"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili pengaturan redaksi yang memungkinkan penyesuaian proses redaksi."
type: docs
weight: 13
url: /id/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

Mewakili pengaturan redaksi, memungkinkan untuk menyesuaikan proses redaksi.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | Menginisialisasi instance baru dari kelas RedactorSettings. |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | Menginisialisasi instance baru dari kelas RedactorSettings dengan instance ILogger yang diberikan. |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | Menginisialisasi instance baru dari kelas RedactorSettings dengan instance IRedactionCallback yang diberikan. |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | Menginisialisasi instance baru dari kelas RedactorSettings dengan instance IOcrConnector yang diberikan. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | Menginisialisasi instance baru dari kelas RedactorSettings dengan instance ILogger dan IRedactionCallback yang diberikan. |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | Menginisialisasi instance baru dari kelas RedactorSettings dengan instance ILogger, IRedactionCallback, dan IOcrConnector yang diberikan. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getLogger()](#getLogger--) | Mendapatkan instance dari sebuah kelas, yang mengimplementasikan |
ILogger
, yang digunakan untuk mencatat peristiwa dan kesalahan.
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | Mengatur instance dari sebuah kelas, yang mengimplementasikan |
ILogger
, yang digunakan untuk mencatat peristiwa dan kesalahan.
|
|  | [getRedactionCallback()](#getRedactionCallback--) | Mendapatkan instance dari sebuah kelas, yang mengimplementasikan |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | Mengatur instance dari sebuah kelas, yang mengimplementasikan |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | Mendapatkan instance dari sebuah kelas, yang mengimplementasikan |
IOcrConnector
antarmuka.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Mengatur instance dari sebuah kelas, yang mengimplementasikan |
IOcrConnector
antarmuka.
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


Menginisialisasi instance baru dari kelas RedactorSettings.


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


Menginisialisasi instance baru dari kelas RedactorSettings dengan instance ILogger yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Sebuah instance dari sebuah kelas, yang mengimplementasikan antarmuka ILogger |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


Menginisialisasi instance baru dari kelas RedactorSettings dengan instance IRedactionCallback yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Sebuah instance dari sebuah kelas, yang mengimplementasikan antarmuka IRedactionCallbck |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


Menginisialisasi instance baru dari kelas RedactorSettings dengan instance IOcrConnector yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Implementasi yang valid dari antarmuka IOcrConnector |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


Menginisialisasi instance baru dari kelas RedactorSettings dengan instance ILogger dan IRedactionCallback yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Sebuah instance dari sebuah kelas, yang mengimplementasikan antarmuka ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Sebuah instance dari sebuah kelas, yang mengimplementasikan antarmuka IRedactionCallbck |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


Menginisialisasi instance baru dari kelas RedactorSettings dengan instance ILogger, IRedactionCallback, dan IOcrConnector yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Sebuah instance dari sebuah kelas, yang mengimplementasikan antarmuka ILogger |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Sebuah instance dari sebuah kelas, yang mengimplementasikan antarmuka IRedactionCallbck |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Sebuah instance dari implementasi antarmuka IOcrConnector. Bisa bernilai null |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Mendapatkan instance dari sebuah kelas, yang mengimplementasikan
ILogger
, yang digunakan untuk mencatat peristiwa dan kesalahan.


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


Mengatur instance dari sebuah kelas, yang mengimplementasikan
ILogger
, yang digunakan untuk mencatat peristiwa dan kesalahan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | Sebuah instance dari sebuah kelas, yang mengimplementasikan ILogger, yang digunakan untuk mencatat peristiwa dan kesalahan. |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


Mendapatkan instance dari sebuah kelas, yang mengimplementasikan
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


Mengatur instance dari sebuah kelas, yang mengimplementasikan
IRedactionCallback
.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | Sebuah instance dari sebuah kelas, yang mengimplementasikan IRedactionCallback. |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Mendapatkan instance dari sebuah kelas, yang mengimplementasikan
IOcrConnector
antarmuka.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Mengatur instance dari sebuah kelas, yang mengimplementasikan
IOcrConnector
antarmuka.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Sebuah instance dari sebuah kelas, yang mengimplementasikan antarmuka IOcrConnector. |
|

