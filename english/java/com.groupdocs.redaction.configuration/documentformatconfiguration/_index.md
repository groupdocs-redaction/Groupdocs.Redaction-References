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
| [getExtensionFilter()](#getExtensionFilter--) | Gets a comma (",") delimited list of file extensions (for example ".pdf"), case insensitive. |
| [setExtensionFilter(String value)](#setExtensionFilter-java.lang.String-) | Sets a comma (",") delimited list of file extensions (for example ".pdf"), case insensitive. |
| [getDocumentType()](#getDocumentType--) | Gets the type of a class, inheriting from  DocumentFormatInstance . |
| [setDocumentType(Class value)](#setDocumentType-java.lang.Class-) | Sets the type of a class, inheriting from  DocumentFormatInstance . |
| [getInitializationData()](#getInitializationData--) | Gets data, required for  DocumentFormatInstance  initialization. |
| [setInitializationData(System.Collections.Generic.Dictionary<String,String> value)](#setInitializationData-com.aspose.ms.System.Collections.Generic.Dictionary-java.lang.String-java.lang.String--) | Sets data, required for  DocumentFormatInstance  initialization. |
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


Gets a comma (",") delimited list of file extensions (for example ".pdf"), case insensitive.

**Returns:**
java.lang.String - A comma (",") delimited list of file extensions (for example ".pdf"), case insensitive.
### setExtensionFilter(String value) {#setExtensionFilter-java.lang.String-}
```
public final void setExtensionFilter(String value)
```


Sets a comma (",") delimited list of file extensions (for example ".pdf"), case insensitive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | A comma (",") delimited list of file extensions (for example ".pdf"), case insensitive. |

### getDocumentType() {#getDocumentType--}
```
public final Class getDocumentType()
```


Gets the type of a class, inheriting from  DocumentFormatInstance .

**Returns:**
java.lang.Class - The type of a class, inheriting from  DocumentFormatInstance .
### setDocumentType(Class value) {#setDocumentType-java.lang.Class-}
```
public final void setDocumentType(Class value)
```


Sets the type of a class, inheriting from  DocumentFormatInstance .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Class | The type of a class, inheriting from  DocumentFormatInstance . |

### getInitializationData() {#getInitializationData--}
```
public final System.Collections.Generic.Dictionary<String,String> getInitializationData()
```


Gets data, required for  DocumentFormatInstance  initialization.

**Returns:**
com.aspose.ms.System.Collections.Generic.Dictionary<java.lang.String,java.lang.String> - Data, required for  DocumentFormatInstance  initialization.
### setInitializationData(System.Collections.Generic.Dictionary<String,String> value) {#setInitializationData-com.aspose.ms.System.Collections.Generic.Dictionary-java.lang.String-java.lang.String--}
```
public final void setInitializationData(System.Collections.Generic.Dictionary<String,String> value)
```


Sets data, required for  DocumentFormatInstance  initialization.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.ms.System.Collections.Generic.Dictionary<java.lang.String,java.lang.String> | Data, required for  DocumentFormatInstance  initialization. |

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
