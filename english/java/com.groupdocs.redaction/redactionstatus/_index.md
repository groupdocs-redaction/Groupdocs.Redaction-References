---
title: RedactionStatus
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a redaction completion status.
type: docs
weight: 20
url: /java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

Represents a redaction completion status.
## Fields

| Field | Description |
| --- | --- |
| [Applied](#Applied) | Redaction was fully and successfully applied. |
| [PartiallyApplied](#PartiallyApplied) | Redaction was aplied only to a part of its matches. |
| [Skipped](#Skipped) | Redaction was skipped (not applied). |
| [Failed](#Failed) | Redaction failed with exception. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


Redaction was fully and successfully applied.

### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


Redaction was aplied only to a part of its matches.

### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


Redaction was skipped (not applied).

### Failed {#Failed}
```
public static final RedactionStatus Failed
```


Redaction failed with exception.

### values() {#values--}
```
public static RedactionStatus[] values()
```




**Returns:**
com.groupdocs.redaction.RedactionStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionStatus valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
