---
title: RedactorLogEntry
second_title: GroupDocs.Redaction for Java API Reference
description: Represents results of applying redaction.
type: docs
weight: 18
url: /java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

Represents results of applying redaction.

--------------------

**Learn more**

 *  More details about redaction log entries: [Redaction basics][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
## Constructors

| Constructor | Description |
| --- | --- |
| [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | Initializes a new instance of RedactorLogEntry class for redaction. |
## Methods

| Method | Description |
| --- | --- |
| [getResult()](#getResult--) | Gets the result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance . |
| [getRedaction()](#getRedaction--) | Gets the reference to redaction and its options. |
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


Initializes a new instance of RedactorLogEntry class for redaction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Reference to redaction |
| result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | Redaction result, reported by format handler |

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


Gets the result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .
### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


Gets the reference to redaction and its options.

**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.
