---
title: IRasterizableDocument
second_title: GroupDocs.Redaction for Java API Reference
description: Defines methods that are required for saving document in any binary form.
type: docs
weight: 26
url: /java/com.groupdocs.redaction.integration/irasterizabledocument/
---```
public interface IRasterizableDocument
```

Defines methods that are required for saving document in any binary form. Built-in types save a document as a PDF with images of its pages.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about saving document as a rasterized PDF: [Save in rasterized PDF][]
 *  More details about rasterization options: [Select specific pages for rasterized PDF][]
 *  More details about implementing custom formats: [Create custom format handler][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Save in rasterized PDF]: https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/
[Select specific pages for rasterized PDF]: https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/
[Create custom format handler]: https://docs.groupdocs.com/redaction/java/create-custom-format-handler/
## Methods

| Method | Description |
| --- | --- |
| [rasterize(OutputStream output)](#rasterize-java.io.OutputStream-) | Saves the document to a stream as a PDF. |
| [rasterize(OutputStream output, RasterizationOptions options)](#rasterize-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | Saves the document to a stream as a PDF with page range and compliance options. |
### rasterize(OutputStream output) {#rasterize-java.io.OutputStream-}
```
public abstract void rasterize(OutputStream output)
```


Saves the document to a stream as a PDF.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Target stream |

### rasterize(OutputStream output, RasterizationOptions options) {#rasterize-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public abstract void rasterize(OutputStream output, RasterizationOptions options)
```


Saves the document to a stream as a PDF with page range and compliance options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Target stream |
| options | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | PDF conversion options |

