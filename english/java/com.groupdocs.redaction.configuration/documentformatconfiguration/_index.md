---
title: DocumentFormatConfiguration
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a type reference for DocumentFormatInstance-derived class and supported file extensions list for faster format detection.
type: docs
weight: 10
url: /java/com.groupdocs.redaction.configuration/documentformatconfiguration/
---
**Inheritance:**
java.lang.Object
```
public class DocumentFormatConfiguration
```

Represents a type reference for  DocumentFormatInstance -derived class and supported file extensions list for faster format detection.

--------------------

**Learn more**

 *  More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list][]
 *  More details about implementing custom formats: [Create custom format handler][]

The following example demonstrates how to set properties for a custom format configuration.

```

  DocumentFormatConfiguration adobePhotoshopSettings = new DocumentFormatConfiguration();
 adobePhotoshopSettings.setExtensionFilter(".psd");
 adobePhotoshopSettings.setDocumentType(MyAdobePhotoshopFormatInstance.class);
 
```


[Extend supported extensions list]: https://docs.groupdocs.com/redaction/java/extend-supported-extensions-list/
[Create custom format handler]: https://docs.groupdocs.com/redaction/java/create-custom-format-handler/
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentFormatConfiguration()](#DocumentFormatConfiguration--) | Initializes a new instance of DocumentFormatConfiguration class. |
## Methods

| Method | Description |
| --- | --- |
| [getExtensionFilter()](#getExtensionFilter--) | Gets or sets a comma (",") delimited list of file extensions (for example ".pdf"), case insensitive. |
| [setExtensionFilter(String value)](#setExtensionFilter-java.lang.String-) | Gets or sets a comma (",") delimited list of file extensions (for example ".pdf"), case insensitive. |
| [getDocumentType()](#getDocumentType--) | Gets or sets the type of a class, inheriting from [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance). |
| [setDocumentType(Class value)](#setDocumentType-java.lang.Class-) | Gets or sets the type of a class, inheriting from [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance). |
| [getInitializationData()](#getInitializationData--) | Gets or sets data, required for [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) initialization. |
| [setInitializationData(System.Collections.Generic.Dictionary<String,String> value)](#setInitializationData-com.aspose.ms.System.Collections.Generic.Dictionary-java.lang.String-java.lang.String--) | Gets or sets data, required for [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) initialization. |
| [supportsExtension(String fileExtension)](#supportsExtension-java.lang.String-) | Checks if a given file extension can be handled as DocumentType. |
### DocumentFormatConfiguration() {#DocumentFormatConfiguration--}
```
public DocumentFormatConfiguration()
```


Initializes a new instance of DocumentFormatConfiguration class.

### getExtensionFilter() {#getExtensionFilter--}
```
public final String getExtensionFilter()
```


Gets or sets a comma (",") delimited list of file extensions (for example ".pdf"), case insensitive.

**Returns:**
java.lang.String
### setExtensionFilter(String value) {#setExtensionFilter-java.lang.String-}
```
public final void setExtensionFilter(String value)
```


Gets or sets a comma (",") delimited list of file extensions (for example ".pdf"), case insensitive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### getDocumentType() {#getDocumentType--}
```
public final Class getDocumentType()
```


Gets or sets the type of a class, inheriting from [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance).

**Returns:**
java.lang.Class
### setDocumentType(Class value) {#setDocumentType-java.lang.Class-}
```
public final void setDocumentType(Class value)
```


Gets or sets the type of a class, inheriting from [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Class |  |

### getInitializationData() {#getInitializationData--}
```
public final System.Collections.Generic.Dictionary<String,String> getInitializationData()
```


Gets or sets data, required for [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) initialization.

**Returns:**
com.aspose.ms.System.Collections.Generic.Dictionary<java.lang.String,java.lang.String>
### setInitializationData(System.Collections.Generic.Dictionary<String,String> value) {#setInitializationData-com.aspose.ms.System.Collections.Generic.Dictionary-java.lang.String-java.lang.String--}
```
public final void setInitializationData(System.Collections.Generic.Dictionary<String,String> value)
```


Gets or sets data, required for [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) initialization.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.ms.System.Collections.Generic.Dictionary<java.lang.String,java.lang.String> |  |

### supportsExtension(String fileExtension) {#supportsExtension-java.lang.String-}
```
public final boolean supportsExtension(String fileExtension)
```


Checks if a given file extension can be handled as DocumentType.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileExtension | java.lang.String | File extension, format is ".ext" |

**Returns:**
boolean - True if the extension is listed in ExtensionFilter
