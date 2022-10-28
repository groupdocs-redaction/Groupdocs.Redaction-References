---
title: Redaction
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a base abstract class for all redaction types.
type: docs
weight: 13
url: /java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

Represents a base abstract class for all redaction types.

--------------------

**Learn more**

 *  More details about redaction types: [Redaction basics][]
 *  More advanced redaction topics: [Advanced usage][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Advanced usage]: https://docs.groupdocs.com/redaction/java/advanced-usage/
## Constructors

| Constructor | Description |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDescription()](#getDescription--) | Returns a string, describing the redaction and its parameters. |
| [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applies the redaction to a given format instance. |
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


Returns a string, describing the redaction and its parameters.

**Returns:**
java.lang.String - Text, containing redaction name and parameters.
### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applies the redaction to a given format instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | An instance of a document to apply redaction |

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any
