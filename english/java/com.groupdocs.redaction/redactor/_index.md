---
title: Redactor
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a main class that controls document redaction process allowing to open redact and save documents.
type: docs
weight: 16
url: /java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

Represents a main class that controls document redaction process, allowing to open, redact and save documents.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More advanced redaction topics: [Advanced usage][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Advanced usage]: https://docs.groupdocs.com/redaction/java/advanced-usage/
## Constructors

| Constructor | Description |
| --- | --- |
| [Redactor(String filePath)](#Redactor-java.lang.String-) | Initializes a new instance of  Redactor  class using file path. |
| [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | Initializes a new instance of  Redactor  class using stream. |
| [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | Initializes a new instance of  Redactor  class for a password-protected document using its path. |
| [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Initializes a new instance of  Redactor  class for a password-protected document using its path and settings. |
| [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | Initializes a new instance of  Redactor  class for a password-protected document using stream. |
| [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Initializes a new instance of  Redactor  class for a password-protected document using stream and settings. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | Releases resources. |
| [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | Applies a redaction to the document. |
| [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | Applies a set of redactions to the document. |
| [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | Applies a redaction policy to the document. |
| [save()](#save--) | Saves the document to a file with the following options: AddSuffix = true, RasterizeToPDF = true. |
| [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | Saves the document to a file. |
| [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | Saves the document to a stream, including custom location. |
| [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | Generates preview images of specific pages in a given image format. |
| [getDocumentInfo()](#getDocumentInfo--) | Gets the general information about the document - size, page count, etc. |
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


Initializes a new instance of  Redactor  class using file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Path to the file

The following example demonstrates how to open a document for redaction.

```

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
     // Here we can use document instance to perform redactions
 }
 
``` |

### Redactor(InputStream document) {#Redactor-java.io.InputStream-}
```
public Redactor(InputStream document)
```


Initializes a new instance of  Redactor  class using stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source stream of the document

The following example demonstrates how to open a document from stream.

```

  try (InputStream stream = new FileInputStream("C:\\sample.pdf"))
 {
     try (Redactor redactor = new Redactor(stream))
     {
         // Here we can use document instance to perform redactions
     }
 }
 
``` |

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


Initializes a new instance of  Redactor  class for a password-protected document using its path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Path to file. |
| loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Options, including password. |

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


Initializes a new instance of  Redactor  class for a password-protected document using its path and settings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Path to file. |
| loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | File-dependent options, including password. |
| settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Default settings for redaction process. |

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


Initializes a new instance of  Redactor  class for a password-protected document using stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source input stream. |
| loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Options, including password. |

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


Initializes a new instance of  Redactor  class for a password-protected document using stream and settings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source input stream. |
| loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Options, including password. |
| settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Default settings for redaction process. |

### close() {#close--}
```
public final void close()
```


Releases resources.

### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


Applies a redaction to the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| redaction | [Redaction](../../com.groupdocs.redaction/redaction) | An instance of  Redaction  to apply |

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case
### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


Applies a set of redactions to the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | An array of redactions to apply |

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case
### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


Applies a redaction policy to the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | Redaction policy |

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case
### save() {#save--}
```
public final String save()
```


Saves the document to a file with the following options: AddSuffix = true, RasterizeToPDF = true.

**Returns:**
java.lang.String - Path to redacted document
### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


Saves the document to a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Options to add suffix or rasterize |

**Returns:**
java.lang.String - Path to redacted document
### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


Saves the document to a stream, including custom location.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.OutputStream | Target stream |
| rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | Options to rasterize or not and to specify pages for rasterization |

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


Generates preview images of specific pages in a given image format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | Image properties and page range settings |

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


Gets the general information about the document - size, page count, etc.

**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo
