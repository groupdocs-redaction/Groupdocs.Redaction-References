---
title: "ILogger"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "रेडैक्शन प्रक्रिया में घटनाओं और त्रुटियों को लॉग करने के लिए उपयोग किए जा सकने वाले लॉगर के इंटरफ़ेस को परिभाषित करता है।"
type: docs
weight: 17
url: /hi/java/com.groupdocs.redaction.options/ilogger/
---```
public interface ILogger
```

Defines interface of a logger that can be used for logging events and errors in process of redaction.

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)

<br />


## Methods

| Method | Description |
| --- | --- |
| [error(String message)](#error-java.lang.String-) | Logs an error that occurred during redaction process.
 |
| [trace(String message)](#trace-java.lang.String-) | Logs an event that occurred during redaction process.
 |
| [warning(String message)](#warning-java.lang.String-) | Logs a warning that occurred during redaction process.
 |
### error(String message) {#error-java.lang.String-}
```
public abstract void error(String message)
```


Logs an error that occurred during redaction process.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The error message.
 |

### trace(String message) {#trace-java.lang.String-}
```
public abstract void trace(String message)
```


Logs an event that occurred during redaction process.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The event message.
 |

### warning(String message) {#warning-java.lang.String-}
```
public abstract void warning(String message)
```


Logs a warning that occurred during redaction process.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The warning message.
 |

