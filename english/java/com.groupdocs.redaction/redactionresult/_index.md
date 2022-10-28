---
title: RedactionResult
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a result of the redaction operation.
type: docs
weight: 15
url: /java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

Represents a result of the redaction operation.

--------------------

**Learn more**

 *  More details about redaction results: [Redaction basics][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
## Methods

| Method | Description |
| --- | --- |
| [getStatus()](#getStatus--) | Gets the execution status. |
| [getErrorMessage()](#getErrorMessage--) | Gets the error message for diagnostics. |
| [skipped(String description)](#skipped-java.lang.String-) | Initializes a new instance of RedactionResult class with Skipped status. |
| [partial(String description)](#partial-java.lang.String-) | Initializes a new instance of RedactionResult class with PartiallyApplied status. |
| [failed(String description)](#failed-java.lang.String-) | Initializes a new instance of RedactionResult class with Failed status. |
| [successful()](#successful--) | Initializes a new instance of RedactionResult class with Applied (successful) status. |
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Gets the execution status.

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.
### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


Gets the error message for diagnostics.

**Returns:**
java.lang.String - The error message for diagnostics.
### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


Initializes a new instance of RedactionResult class with Skipped status.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| description | java.lang.String | Reason why the operation was skipped |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result
### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


Initializes a new instance of RedactionResult class with PartiallyApplied status.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| description | java.lang.String | Reason why the operation was not fully applied |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result
### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


Initializes a new instance of RedactionResult class with Failed status.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| description | java.lang.String | Failure or exception details |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result
### successful() {#successful--}
```
public static RedactionResult successful()
```


Initializes a new instance of RedactionResult class with Applied (successful) status.

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result
