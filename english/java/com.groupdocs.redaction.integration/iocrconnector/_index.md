---
title: IOcrConnector
second_title: GroupDocs.Redaction for Java API Reference
description: Defines methods that are required to apply textual redactions to image documents and embedded images.
type: docs
weight: 23
url: /java/com.groupdocs.redaction.integration/iocrconnector/
---```
public interface IOcrConnector
```

Defines methods that are required to apply textual redactions to image documents and embedded images.

--------------------

**Learn more**

 *  More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics][]
 *  An example of implementation using Aspose.OCR for Cloud: [Use Aspose.OCR for Cloud SDK][]
 *  An example of implementation using Microsoft Azure Cognitive Services: [Use Microsoft Azure ComputerVision REST API][]


[OCR Usage Basics]: https://docs.groupdocs.com/redaction/java/ocr-usage-basics/
[Use Aspose.OCR for Cloud SDK]: https://docs.groupdocs.com/redaction/java/use-aspose-ocr-for-cloud/
[Use Microsoft Azure ComputerVision REST API]: https://docs.groupdocs.com/redaction/java/use-microsoft-azure-computer-vision/
## Methods

| Method | Description |
| --- | --- |
| [recognize(InputStream imageStream)](#recognize-java.io.InputStream-) | Does the OCR processing of an image, provided as a stream. |
### recognize(InputStream imageStream) {#recognize-java.io.InputStream-}
```
public abstract RecognizedImage recognize(InputStream imageStream)
```


Does the OCR processing of an image, provided as a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageStream | java.io.InputStream | Stream, containing an image to process |

**Returns:**
[RecognizedImage](../../com.groupdocs.redaction.integration/recognizedimage) - Structured recognized text, containing lines, words and their bounding rectangles
