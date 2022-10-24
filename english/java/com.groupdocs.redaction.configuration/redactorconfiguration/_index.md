---
title: RedactorConfiguration
second_title: GroupDocs.Redaction for Java API Reference
description: Provides access to a list of supported formats built-in and custom user formats.
type: docs
weight: 11
url: /java/com.groupdocs.redaction.configuration/redactorconfiguration/
---
**Inheritance:**
java.lang.Object
```
public class RedactorConfiguration
```

Provides access to a list of supported formats, built-in and custom user formats.

--------------------

**Learn more**

 *  More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list][]
 *  More details about implementing custom formats: [Create custom format handler][]

The following example demonstrates how to add a custom user format handler.

```

  DocumentFormatConfiguration adobePhotoshopSettings = new DocumentFormatConfiguration();
 adobePhotoshopSettings.setExtensionFilter(".psd");
 adobePhotoshopSettings.setDocumentType(MyAdobePhotoshopFormatInstance.class);
 RedactorConfiguration configuration = RedactorConfiguration.getInstance();
 configuration.getAvailableFormats().add(adobePhotoshopSettings);
 
```


[Extend supported extensions list]: https://docs.groupdocs.com/redaction/java/extend-supported-extensions-list/
[Create custom format handler]: https://docs.groupdocs.com/redaction/java/create-custom-format-handler/
## Constructors

| Constructor | Description |
| --- | --- |
| [RedactorConfiguration()](#RedactorConfiguration--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getAvailableFormats()](#getAvailableFormats--) | Gets a list of recognized formats, see  DocumentFormatConfiguration . |
| [findFormat(String fileExtension)](#findFormat-java.lang.String-) | Finds format configurations for a given file extension. |
### RedactorConfiguration() {#RedactorConfiguration--}
```
public RedactorConfiguration()
```


### getAvailableFormats() {#getAvailableFormats--}
```
public final List<DocumentFormatConfiguration> getAvailableFormats()
```


Gets a list of recognized formats, see  DocumentFormatConfiguration .

**Returns:**
java.util.List<com.groupdocs.redaction.configuration.DocumentFormatConfiguration> - A list of recognized formats, see  DocumentFormatConfiguration .
### findFormat(String fileExtension) {#findFormat-java.lang.String-}
```
public final DocumentFormatConfiguration findFormat(String fileExtension)
```


Finds format configurations for a given file extension.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileExtension | java.lang.String | File extension, format is ".ext" |

**Returns:**
[DocumentFormatConfiguration](../../com.groupdocs.redaction.configuration/documentformatconfiguration) - If found, instance of  DocumentFormatConfiguration , null otherwise
