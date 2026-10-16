---
title: "ILogger"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "Redaction 과정에서 이벤트와 오류를 기록하는 데 사용할 수 있는 로거 인터페이스를 정의합니다."
type: docs
weight: 17
url: /ko/java/com.groupdocs.redaction.options/ilogger/
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

