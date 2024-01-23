---
title: RedactionActionType
second_title: GroupDocs.Redaction for Java API Reference
description: Represents actions that can be taken to perform redaction.
type: docs
weight: 34
url: /java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

Represents actions that can be taken to perform redaction.
## Fields

| Field | Description |
| --- | --- |
| [Replacement](#Replacement) | Redacted text was replaced with another or covered with a block. |
| [Cleanup](#Cleanup) | Data were removed, but an empty object remains in the document. |
| [Deletion](#Deletion) | Data and related structures were removed from the document. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


Redacted text was replaced with another or covered with a block.

### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


Data were removed, but an empty object remains in the document.

### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


Data and related structures were removed from the document.

### values() {#values--}
```
public static RedactionActionType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.RedactionActionType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionActionType valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
