---
title: TextRedaction
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a base abstract class for document text redactions.
type: docs
weight: 25
url: /java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

Represents a base abstract class for document text redactions.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about document text redactions: [Text redactions][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Text redactions]: https://docs.groupdocs.com/redaction/java/text-redactions/
## Methods

| Method | Description |
| --- | --- |
| [getActionOptions()](#getActionOptions--) | Gets the  ReplacementOptions  instance, specifying type of text replacement. |
| [getOcrConnector()](#getOcrConnector--) | Gets the  IOcrConnector  implementation, required to extract text from graphic content. |
| [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Sets the  IOcrConnector  implementation, required to extract text from graphic content. |
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


Gets the  ReplacementOptions  instance, specifying type of text replacement.

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.
### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Gets the  IOcrConnector  implementation, required to extract text from graphic content.

**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.
### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Sets the  IOcrConnector  implementation, required to extract text from graphic content.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | The  IOcrConnector  implementation, required to extract text from graphic content. |

