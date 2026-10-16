---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "रेडैक्शन प्रक्रिया को अनुकूलित करने की अनुमति देने वाले रेडैक्शन सेटिंग्स का प्रतिनिधित्व करता है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

रेडैक्शन सेटिंग्स को दर्शाता है, जिससे रेडैक्शन प्रक्रिया को अनुकूलित किया जा सकता है।

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | RedactorSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | दिए गए ILogger इंस्टेंस के साथ RedactorSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | दिए गए IRedactionCallback इंस्टेंस के साथ RedactorSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | दिए गए IOcrConnector इंस्टेंस के साथ RedactorSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | दिए गए ILogger और IRedactionCallback इंस्टेंस के साथ RedactorSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | दिए गए ILogger, IRedactionCallback और IOcrConnector इंस्टेंस के साथ RedactorSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getLogger()](#getLogger--) | किसी क्लास का एक इंस्टेंस प्राप्त करता है, जो लागू करता है |
ILogger
, जो इवेंट्स और त्रुटियों को लॉग करने के लिए उपयोग किया जाता है।
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | किसी क्लास का एक इंस्टेंस सेट करता है, जो लागू करता है |
ILogger
, जो इवेंट्स और त्रुटियों को लॉग करने के लिए उपयोग किया जाता है।
|
|  | [getRedactionCallback()](#getRedactionCallback--) | किसी क्लास का एक इंस्टेंस प्राप्त करता है, जो लागू करता है |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | किसी क्लास का एक इंस्टेंस सेट करता है, जो लागू करता है |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | किसी क्लास का एक इंस्टेंस प्राप्त करता है, जो लागू करता है |
IOcrConnector
इंटरफ़ेस।
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | किसी क्लास का एक इंस्टेंस सेट करता है, जो लागू करता है |
IOcrConnector
इंटरफ़ेस।
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


RedactorSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


दिए गए ILogger इंस्टेंस के साथ RedactorSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | एक क्लास का इंस्टेंस, जो ILogger इंटरफ़ेस को लागू करता है |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


दिए गए IRedactionCallback इंस्टेंस के साथ RedactorSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | एक क्लास का इंस्टेंस, जो IRedactionCallbck इंटरफ़ेस को लागू करता है |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


दिए गए IOcrConnector इंस्टेंस के साथ RedactorSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector इंटरफ़ेस का एक वैध कार्यान्वयन |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


दिए गए ILogger और IRedactionCallback इंस्टेंस के साथ RedactorSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | एक क्लास का इंस्टेंस, जो ILogger इंटरफ़ेस को लागू करता है |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | एक क्लास का इंस्टेंस, जो IRedactionCallbck इंटरफ़ेस को लागू करता है |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


दिए गए ILogger, IRedactionCallback और IOcrConnector इंस्टेंस के साथ RedactorSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | एक क्लास का इंस्टेंस, जो ILogger इंटरफ़ेस को लागू करता है |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | एक क्लास का इंस्टेंस, जो IRedactionCallbck इंटरफ़ेस को लागू करता है |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector इंटरफ़ेस कार्यान्वयन का एक इंस्टेंस। null हो सकता है |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


किसी क्लास का एक इंस्टेंस प्राप्त करता है, जो लागू करता है
ILogger
, जो इवेंट्स और त्रुटियों को लॉग करने के लिए उपयोग किया जाता है।


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


किसी क्लास का एक इंस्टेंस सेट करता है, जो लागू करता है
ILogger
, जो इवेंट्स और त्रुटियों को लॉग करने के लिए उपयोग किया जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | एक क्लास का इंस्टेंस, जो  ILogger को लागू करता है, जो इवेंट्स और त्रुटियों को लॉग करने के लिए उपयोग किया जाता है। |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


किसी क्लास का एक इंस्टेंस प्राप्त करता है, जो लागू करता है
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


किसी क्लास का एक इंस्टेंस सेट करता है, जो लागू करता है
IRedactionCallback
.


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | एक क्लास का इंस्टेंस, जो  IRedactionCallback को लागू करता है। |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


किसी क्लास का एक इंस्टेंस प्राप्त करता है, जो लागू करता है
IOcrConnector
इंटरफ़ेस।


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


किसी क्लास का एक इंस्टेंस सेट करता है, जो लागू करता है
IOcrConnector
इंटरफ़ेस।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | एक क्लास का इंस्टेंस, जो  IOcrConnector इंटरफ़ेस को लागू करता है। |
|

