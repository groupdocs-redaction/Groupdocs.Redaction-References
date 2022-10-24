---
title: RedactorChangeLog
second_title: GroupDocs.Redaction for Java API Reference
description: Represents results for a list of redactions passed to Apply method of Redactor class.
type: docs
weight: 17
url: /java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Represents results for a list of redactions, passed to Apply() method of  Redactor  class.

--------------------

**Learn more**

 *  More details about redaction logs: [Redaction basics][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
## Constructors

| Constructor | Description |
| --- | --- |
| [RedactorChangeLog()](#RedactorChangeLog--) | Initializes a new instance of RedactorChangeLog class. |
## Methods

| Method | Description |
| --- | --- |
| [getStatus()](#getStatus--) | Gets the final status of all applied redactions. |
| [getRedactionLog()](#getRedactionLog--) | Gets the list of  RedactorLogEntry  instances. |
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


Initializes a new instance of RedactorChangeLog class.

### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Gets the final status of all applied redactions.

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.
### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


Gets the list of  RedactorLogEntry  instances.

**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - The list of  RedactorLogEntry  instances.
