---
title: DocumentFormatInstance
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a specific format of a document.
type: docs
weight: 10
url: /java/com.groupdocs.redaction.integration/documentformatinstance/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFormatInstance
```

Represents a specific format of a document. Implement this class to add your own document types.

--------------------

**Learn more**

 *  More details about implementing custom formats: [Create custom format handler][]

The following example demonstrates how to create an empty stub for a custom format handler.

```

  public class DummyDocument extends DocumentFormatInstance
 {     
     {@literal @}Override
     public void load(InputStream output) throws java.lang.Exception
     {
         // load file content
     }
     {@literal @}Override
     public void save(OutputStream output) throws java.lang.Exception
     {
         // save changes to file;
     }
 }
 
```


[Create custom format handler]: https://docs.groupdocs.com/redaction/java/create-custom-format-handler/
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentFormatInstance()](#DocumentFormatInstance--) |  |
## Methods

| Method | Description |
| --- | --- |
| [createInstance(Class docType)](#createInstance-java.lang.Class-) |  |
| [getPassword()](#getPassword--) | Gets a password for password protected documents. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Sets a password for password protected documents. |
| [getRequiresRasterization()](#getRequiresRasterization--) | Gets value, indicating if the format instance is read-only and cannot be saved in original format. |
| [isAccessGranted()](#isAccessGranted--) |  |
| [initialize(DocumentFormatConfiguration config, RedactorSettings settings)](#initialize-com.groupdocs.redaction.configuration.DocumentFormatConfiguration-com.groupdocs.redaction.options.RedactorSettings-) | Performs initialization of the instance of document format handler. |
| [load(InputStream input)](#load-java.io.InputStream-) | Loads the document from a stream. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Saves the document to a stream. |
| [isRedactionAccepted(RedactionDescription description)](#isRedactionAccepted-com.groupdocs.redaction.redactions.RedactionDescription-) | Checks for  IRedactionCallback  implementation and invokes it, if specified. |
| [performBinaryCheck(InputStream input)](#performBinaryCheck-java.io.InputStream-) | Checks if the given stream contains a document, supported by this format instance. |
| [getDefaultConfiguration()](#getDefaultConfiguration--) | Provides a singleton instance with default configuration of built-in formats. |
### DocumentFormatInstance() {#DocumentFormatInstance--}
```
public DocumentFormatInstance()
```


### createInstance(Class docType) {#createInstance-java.lang.Class-}
```
public static DocumentFormatInstance createInstance(Class docType)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| docType | java.lang.Class |  |

**Returns:**
[DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance)
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Gets a password for password protected documents.

**Returns:**
java.lang.String - A password for password protected documents.
### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Sets a password for password protected documents.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | A password for password protected documents. |

### getRequiresRasterization() {#getRequiresRasterization--}
```
public boolean getRequiresRasterization()
```


Gets value, indicating if the format instance is read-only and cannot be saved in original format.

**Returns:**
boolean - Value, indicating if the format instance is read-only and cannot be saved in original format.
### isAccessGranted() {#isAccessGranted--}
```
public final boolean isAccessGranted()
```




**Returns:**
boolean
### initialize(DocumentFormatConfiguration config, RedactorSettings settings) {#initialize-com.groupdocs.redaction.configuration.DocumentFormatConfiguration-com.groupdocs.redaction.options.RedactorSettings-}
```
public void initialize(DocumentFormatConfiguration config, RedactorSettings settings)
```


Performs initialization of the instance of document format handler.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| config | [DocumentFormatConfiguration](../../com.groupdocs.redaction.configuration/documentformatconfiguration) | Format configuration |
| settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Default settings for redaction process. |

### load(InputStream input) {#load-java.io.InputStream-}
```
public void load(InputStream input)
```


Loads the document from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| input | java.io.InputStream | Stream to read from |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream output)
```


Saves the document to a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Target stream to save the document |

### isRedactionAccepted(RedactionDescription description) {#isRedactionAccepted-com.groupdocs.redaction.redactions.RedactionDescription-}
```
public final boolean isRedactionAccepted(RedactionDescription description)
```


Checks for  IRedactionCallback  implementation and invokes it, if specified.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| description | [RedactionDescription](../../com.groupdocs.redaction.redactions/redactiondescription) | Redaction description |

**Returns:**
boolean - True (by default) if redaction is accepted
### performBinaryCheck(InputStream input) {#performBinaryCheck-java.io.InputStream-}
```
public boolean performBinaryCheck(InputStream input)
```


Checks if the given stream contains a document, supported by this format instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| input | java.io.InputStream | Document content stream |

**Returns:**
boolean - True, if the document can be loaded by this format instance and false otherwise
### getDefaultConfiguration() {#getDefaultConfiguration--}
```
public static RedactorConfiguration getDefaultConfiguration()
```


Provides a singleton instance with default configuration of built-in formats.

**Returns:**
[RedactorConfiguration](../../com.groupdocs.redaction.configuration/redactorconfiguration) - Configuration instance
