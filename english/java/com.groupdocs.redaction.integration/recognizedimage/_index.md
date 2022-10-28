---
title: RecognizedImage
second_title: GroupDocs.Redaction for Java API Reference
description: Represents text extracted from an image as a result of its recognition process.
type: docs
weight: 13
url: /java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

Represents text, extracted from an image as a result of its recognition process.

--------------------

**Learn more**

 *  More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics][]


[OCR Usage Basics]: https://docs.groupdocs.com/redaction/java/ocr-usage-basics/
## Constructors

| Constructor | Description |
| --- | --- |
| [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | Initializes a new instance of the class, using a set of recognized lines. |
## Methods

| Method | Description |
| --- | --- |
| [getText()](#getText--) | Gets textual equivalent of the structured text. |
| [getLines()](#getLines--) | Gets lines of text, with their fragments, recognized within the document. |
| [toString()](#toString--) | Gets textual equivalent of the structured text. |
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


Initializes a new instance of the class, using a set of recognized lines.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | an IEnumerable (e.g. a list or an array) of recognized lines |

### getText() {#getText--}
```
public final String getText()
```


Gets textual equivalent of the structured text.

**Returns:**
java.lang.String - Textual equivalent of the structured text.
### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


Gets lines of text, with their fragments, recognized within the document.

**Returns:**
com.groupdocs.redaction.integration.TextLine[] - Lines of text, with their fragments, recognized within the document.
### toString() {#toString--}
```
public String toString()
```


Gets textual equivalent of the structured text.

**Returns:**
java.lang.String - Recognized text
